# Serverless project for S3 bucket website

As part of the cloud resume challenge, there is a need to create ann S3 bucket to host a static website.

I have chosen to use the Serverless framework here because it is the tool I am most familiar with at this time.

## Proposed rules of the bucket

- Allow upload of build files by Github actions
- Allow public viewing of index file over the internet
- Use SSO dev role to interact with the bucket.

## Steps to setup the project

- Install the project dependencies by runnning `npm install`
- Set up the project if it is the first time by running `serverless --org=your_serverless_org_name` and follow the prompts
- Configure Serverless to use the generated SSO profile `sls config credentials -o --provider aws --key change_me --secret change_me --profile serverless`
- To deploy the project run `serverless deploy`
- To tear down the deployment, run `serverless remove`
- Create a serverless framework app
- Run the follwing command to init the serverless project
- Configure the serverless organization
- Deploy the application

## TODO

- Integrate the backend infrastructure
- Use other tools to build and automate the infrastructure (AWS SAM)
