# Continuous deployment pipeline for Lumen / Laravel applications using GitLab and AWS Elastic Beanstalk

Comprehensive description / tutorial may be added in the future.
For now, feel free to use the provided files and adapt them to your requirements.

## Mini tutorial
- Set up a new application in AWS EB, create two environments "staging" and "production"
- Put environment specific environment properties in the EB environment settings, for example "APP_ENV"
- In AWS IAM create a new user and assign the "AWSElasticBeanstalkFullAccess" policy (not quite secure)
- In your GitLab project add two variables "AWS_ACCESS_KEY_ID" and "AWS_SECRET_ACCESS_KEY" with the values from the IAM user
- Push some changes to the master branch of your project and enjoy the magic
