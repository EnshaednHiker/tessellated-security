# Tessellated Security
Tessellated Security is an end-to-end service to take your own tessel 2 and a magnetic switch and build your own security system. 

For the DYI security afficionado, all inclusive code to run a server (Node/Express), webclient, database (MongoDB/Mongoose), and a [tessel](https://tessel.io/) hooked up to a [magnetic door switch](https://www.sparkfun.com/products/13247). A detailed spec sheet of all of the parts used is below along with detailed instructions on how to put what where.  The project's server running here is hosted on Heroku while the database is on mLab. Below is an explanation about setting up your own tessel.

## Server
The server at this time is currently hosted on Heroku. I used CircleCI for continuous integration testing. [Github repo for the server API for the service.](https://github.com/EnshaednHiker/tessellated-security-server) The database for the data layer is hosted on mLab

## Webclient
[Live website for the service.](https://enshaednhiker.github.io/tessellated-security-webclient/) [Github Repo for the client website used to sign up for the service.](https://github.com/EnshaednHiker/tessellated-security-webclient) I used webpack and director as the two chief technologies to make this site.   

## Commandline Package
[Commandline package Github Repo for code to be installed onto a tessel](https://github.com/EnshaednHiker/tessellated-security-command-line-package). I wrote the command line package in node and [published it to NPM](https://www.npmjs.com/package/tessellated-security). As of now, the the only way to get the code on to the tessel is through this npm package. 

## Tutorial

### 1. Spec sheet - gathering the parts you'll need

1. [Tessel](https://www.sparkfun.com/products/13841?ref=tessel.io)
2. [Magnetic Switch](https://www.sparkfun.com/products/13247)
3. [USB micro-B cable](https://www.sparkfun.com/products/10215) (NOTE: most charging cables that come with Android smartphones are USB micro-B cables, so you  might not need to purchase one of these)
4. [USB Power Adapter](https://www.sparkfun.com/products/11456)

### 2. Assembly - putting together the tessel

### 3. Set up an account
 
### 4. Push code to tessel

### 5. Install tessel onto a door

### 6. Demo of the the system in action


