# Hosting a Full-Stack Application

# Udagram

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

### ScreenShots

**AWS RDS for the database overview**

![AWS-RDS](./assets/Screenshot%202025-03-13%20at%2011.20.22 AM.png)
**AWS ElasticBeanstalk for the (backend) API deployment**

![ElasticBeanstalk](./assets/Screenshot%202025-03-16%20at%2012.49.26 AM.png)

**AWS S3 for (frontend) web hosting**

##### Create a new bucket.

![butbucket](./assets/Screenshot%202025-03-13%20at%2011.19.20 AM.png)

##### This screen indicates that the upload of static files was successful.

![butbucket2](./assets/Screenshot%202025-03-13%20at%203.42.22 PM.png)

**Successful CircleCi build**

![alljobs](./assets/Screenshot%202025-03-16%20at%2012.41.44 AM.png)
![build](./assets/Screenshot%202025-03-15%20at%205.40.31 AM.png)
![deploy](./assets/Screenshot%202025-03-15%20at%2010.59.50 PM.png)

**Environment Variables**

![env](./assets/environment_variables.png)

### Domains:

- [FrontEnd Domain](http://mybucket627818603677.s3-website-us-east-1.amazonaws.com/home)
- [Backend Domain](http://udagram-api-dev.us-east-1.elasticbeanstalk.com/)

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
