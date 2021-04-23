# BookingZone API Server
BookingZone’s wants to create a premier platform for multi-entertainment facilities to manage their entertainment options and connect with their consumers.  BookingZone’s Multi-tainment Centre Management System (MCMS) shall provide convenience for vendors to manage their entertainment options and allows consumers the ability to schedule, book and pay for the services.  By connecting consumers directly with venues that have the entertainment options they are looking for and allowing them to have control over their entertainment options.  For the vendor, BookingZone’s MCMS shall allow less time managing schedules, events and payments and allows them more to focus on revenue generating activities.

## Cloud Service
- Persistent 
  - AWS DynamoDB
  - AWS Athena and S3
 - Infracture Language
   - Cloudformation
   - CDK
 - Programming Language
   - TypeScript (Javascript)
   - Node Js (Nest Js Framework)
 - Deployment Architecture
   - Lambda
 
## REST Architecture
There are design rules that are applied to establish the different characteristics of the REST architecture
![Architecture](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/6.png)

## URL Construction
- http://[host]:[port]/api/{service name}]/v{version number}/{resource}
  - An example: http://127.0.0.1/api/v1/users/login
- CRUD actions should be represented by HTTP methods. 
  - Below is the proposed methodology to implement CRUD operations in a RESTful API.

| URL | GET | POST | PUT | DELETE
| ------ | ------ | ------ | ------ |------ |
| /api/v1/category | Yes | Yes | No | No |
| /api/v1/category/{id} | Yes | No | Yes | No |
| /api/v1/category/{id}/business | Yes | Yes | No | No |
| /api/v1/category/{id}/business/{id} | Yes | No | Yes | No |

## API Versioning
- Versioning through URI Path
  - Example:- http://127.0.0.1/api/v1.2.3/user/login
 ![versioning](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/8.jpg)
## Project Dependency installation
- Install node js globally (node version should be >= 12.x)
  ```sh
  sudo apt install nodejs
  check node version (node -v or node –version)
  ```
- Install npm (node package manager) (node version should be >=6.x)
  ```sh
  sudo apt install npm
  check npm version (npm -v or npm –version)
  ```
- Install aws cli sdk globally
  ```sh
  sudo apt-get install awscli
  check aws cli veriosn (aws --version)
  ```
- Install Serverless globally
  ```sh
  npm install -g serverless or npm install serverless -g
  check serverless version (serverless -v)
  ```
- Install Git
  ```sh
  sudo apt install git-all
  check git version (git --version)
  ```
## Project Install
- Clone the repo using ssh
  ```sh
  git clone ssh://bz/v1/repos/bz-api-server
  ```
- Clone the rep using https
  ```sh
  https://git-codecommit.us-east-1.amazonaws.com/v1/repos/bz-api-server
   ```
- Go to project directory 
  ```sh
  cd bz-api-server
  ```
- Run npm install command
  ```sh
   ~bz-api-server$ npm install
   ```
- After install the project dependancy we run the project locally (port 3000)
  ```sh
  ~bz-api-server$ npm run start
   ```
- For build the and deploy the project on server 
  ```sh
  ~bz-api-server$ serverless deploy
  ```
Verify the deployment by navigating to your server address in
your preferred browser.
```sh
127.0.0.1:3000/dev/
```
## Useful links
Here is the links
- [Amazon web service](http://aws.amazon.com/)
- [Node Js](https://nodejs.org/en/)
- [Express Js](https://expressjs.com/)
- [Nest Js](https://nestjs.com/)
- [Serverless](https://www.serverless.com/)
- [npm](https://www.npmjs.com/)
