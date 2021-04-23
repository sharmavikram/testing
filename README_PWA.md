# BookingZone API Server
BookingZone’s wants to create a premier platform for multi-entertainment facilities to manage their entertainment options and connect with their consumers.  BookingZone’s Multi-tainment Centre Management System (MCMS) shall provide convenience for vendors to manage their entertainment options and allows consumers the ability to schedule, book and pay for the services.  By connecting consumers directly with venues that have the entertainment options they are looking for and allowing them to have control over their entertainment options.  For the vendor, BookingZone’s MCMS shall allow less time managing schedules, events and payments and allows them more to focus on revenue generating activities.

## Cloud Service
- Persistent 
  - AWS S3
 - Infracture Language
   - Cloudformation
   - CDK
 - Programming Language
   - TypeScript (Javascript)
   - React Js (Next Js) framework
 - Deployment Architecture
   - Lambda
 
## Serverless web application architecture
![Architecture](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/4.png)

## Progressive web application architecture
![Architecture](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/2.png)
## HTTP Response
- **Successful Response:**
  - **200** : OK, GET POST PUT DELETE
  - **205** : Reset Content
  - **207** : Multi-Status (Conveys information about multiple resources, for situations where multiple status codes might be appropriate.)
  - **208** : Already Reported
- **Client Errors:**
  - **400** : Bad Request
  - **401** : UnAuthorized
  - **402** : Payment Required
  - **403** : Forbidden
  - **404** : Resource Not Found
  - **405** : Method Not Allowed
  - **406** : Not Acceptable
  - **408** : Request timeout
- **Server Error Response:**
  - **500** : Internal server Error
  - **501** : API not implemented
  - **502** : Bad Gateway
  - **503** : Service unavailable
  - **504** : Gateway timeout

## Front-End Technology
We are using react js library for creating front-end progressive web applications using the next js framework. Here is the list of major libraries

| S No. | Libraray | Version |
| ------ | ------ | ------ | 
| 1 | **React Js** | 16.x | 
| 2 | **Typescript** | 4.x | 
| 3 | **Next Js** | 9.5.x | 
| 4 | **React bootstrap** | 1.x | 
| 5 | **Redux** | 4.x | 
| 6 | **Webpack** | 4.x | 
| 7 | **Sass** | 1.x | 
| 8 | **FontAwesome** | 5.x | 

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
  git clone ssh://bz/v1/repos/bz-customer-web
  ```
- Clone the rep using https
  ```sh
  https://git-codecommit.us-east-1.amazonaws.com/v1/repos/bz-customer-web
   ```
- Go to project directory 
  ```sh
  cd bz-customer-web
  ```
- Run npm install command
  ```sh
   ~bz-customer-webr$ npm install
   ```
- After install the project dependancy we run the project locally (port 3000)
  ```sh
  ~bz-customer-webr$ npm run start:dev
   ```
- For build the project
  ```sh
  ~bz-api-server$ npm run build
  ```
- For prettify the code
  ```sh
  ~bz-api-server$ npm run pretty
  ```
Verify the deployment by navigating to your server address in
your preferred browser.
```sh
127.0.0.1:3000
```
## Useful links
Here is the links
- [Amazon web service](http://aws.amazon.com/)
- [Node Js](https://nodejs.org/en/)
- [React Js](https://reactjs.org/)
- [Next Js](https://nextjs.org/)
- [Serverless](https://www.serverless.com/)
- [npm](https://www.npmjs.com/)
