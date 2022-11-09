# Hosting a Full-Stack Application

In order to make a full-stack software created for a store accessible to consumers, I will deploy it to AWS for this repository. I'll utilise Amazon Web Services (AWS) to launch and set up the app's necessary services, such as a database (AWS RDS), a web server (AWS Elastic Beanstalk), and site hosting (AWS S3).

CircleCI has been integrated into this project to automate the pipeline. It will also contain documentation outlining how the deployment process operates. The documentation will be used as a communication guide for all parties participating in this software, including future developers.

## Check the `master` branch's status for CircleCI builds.

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/lone-eagle-youssef/youssef-udagram/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/lone-eagle-youssef/youssef-udagram/tree/master)

https://app.circleci.com/pipelines/github/lone-eagle-youssef/youssef-udagram?branch=master

### Front App Link

http://youssef-udagram.s3-website-us-east-1.amazonaws.com/

### Server Link

http://udagram-api-env.eba-p2rywzj4.us-east-1.elasticbeanstalk.com/

### (Start / Build / Deploy) the programme locally (on the `master` branch)

Create a `.env` file with the following variables inside `udagram-api`:

- POSTGRES_HOST
- POSTGRES_USERNAME
- POSTGRES_PASSWORD
- POSTGRES_DB
- DB_PORT
- PORT
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_REGION
- AWS_PROFILE
- AWS_BUCKET
- URL
- JWT_SECRET

Open `udagram-api` in Terminal and Write The Following:-

```
cd udagram/udagram-api
npm install
npm run dev
npm run build
npm run deploy
```

Open `udagram-frontend` in Terminal and Write The Following:-

```
cd udagram/udagram-frontend
npm install
npm run start
npm run build
npm run deploy
```
