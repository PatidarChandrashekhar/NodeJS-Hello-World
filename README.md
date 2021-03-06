
## Get an API up and running

First, we create a new swagger project and test a simple "NodeJS-Hello-World" API.

## 1. Install swagger, as described as per below:
Installing on Windows
#Open a terminal.

Run the install:
npm install -g swagger

### 2. Create swagger project directory and cd to it. This is where you'll create your first project.

Execute the project create command:

swagger project create hello-world

### 3. Pick the API framework you want to use. We're going to pick express, but you can pick any of the listed frameworks:

#### ? Framework? (Use arrow keys)
####  connect
#### ❯express
####  hapi
####  restify
####  sails

Note: You must enter the number of the option.

swagger creates a skeleton project that's pre-configured to use your selected framework (in this example, Express). It then runs npm install to pick up the dependencies.

Note: Windows users see the note below regarding npm.

Change to the new project directory: cd NodeJS-Hello-World

### 4. Running the project
swagger project start
to start your API. You now have an API running with swagger!

In another terminal, run this command:

curl http://127.0.0.1:10010/hello?name=Scott

And, you'll get back the response { "message": "Hello, Scott!" }.

That's it - You have now created, started and tested your first API project with swagger!

### 5. How to Open the Swagger editor

swagger project edit

### 6. Open project in Visual studio code

C:\SHEKHAR\DEVELOPMENTS\NodeJS\NodeJS-Hello-World>code .


### 7. Open visual studio code directly 

@echo off

CALL "c:\program files\nodejs\nodevars.bat"

Start %ComSpec% /k ""c:\program files\microsoft vs code\code.exe""


### 8. Cloud Foundary CLI for pushing and managing apps, creating and bindinng services

1. Get help in the CLI:
$ cf help

2. Logging to the CLI: 
$ cf login -a https://api.example.com
OR $ cf login -a https://api.example.com -u username@example.com -o example-org -s development
API endpoint: https://api.example.com

3. Push an application:
$ cf push <applicatoin name>
  
CLI refrence: https://docs.cloudfoundry.org/devguide/deploy-apps/deploy-app.html
  
  
### 9. Run NodeJS application from command prompt:
  node [main.js file name without extension] [if any arguments]
  
### 10. Run NodeJS application from batch file:
1. @ECHO Task Name: Hospital Management System
2. @ECHO Login to PCF
3. cf login -a https://api.sys.cf.com -u username -p password -o HMS -s HMS_Production
4. @ECHO run task
5. cf run-task HMS-App "node app start" --name "application start" -m 1GB
  
### 11. ECS S3 Storage Parameters:
1. accessKey
2. bucket
3. endpoint
4. path-style-access
5. s3Url
6. secretKey

