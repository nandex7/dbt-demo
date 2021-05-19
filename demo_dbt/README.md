Welcome to your new dbt project!

### Using the starter project
I follow this instructions.

https://www.youtube.com/watch?v=5rNquRnNb4E


1) dbt -version
2) dbt init demo_dbt
3) Change the profiles.yml
Sample :

snowflake:
  target: dev
  outputs:
    dev:
      type: snowflake
      account: kka65045.us-east-1

      # User/password auth
      user: UserXXX
      password: xxxx

      role: ACCOUNTADMIN
      database: DEMO_DB
      warehouse: COMPUTE_WH
      schema: PUBLIC
      threads: 10
      client_session_keep_alive: False
4) Change the profile name  in dbt_project.yml

profile: 'snowflake'.


5) dbt run
6) dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](http://slack.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
