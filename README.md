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

### 2. Set up an account on the web client and add a device to your account

1. Go to the [website](https://enshaednhiker.github.io/tessellated-security-webclient/)
2. Click on "Register" in the nav bar
3. Fill in information to add an account. The email you put in will be the email that you will receive alerts through. The email can be changed later if you wish.
4. Add a device to your account. Give it a name that will be meaningful for the alert you receive. For instance, if you gave your device the name "back door," the alert you'll receive from that device will be "Alert: the back door opened."
5. Copy the token that gets generated by the site. This token is used later in setting up code on the tessel.

Note: say you add a device your account in the website, set up a tessel with that generated token, and then install a token on a door. If you delete your device in your accout, that will render that device useless, and you'll need to add a new device your account, push code again to the tessel with the newly generated token, and then reinstall the token on your door.

Watch the video from 0:00 to 2:30 for a comprehensive walkthrough on using the website.

### 3. Assembly - putting together the tessel

Watch the video from 2:31 to 3:20 for a comprehensive walthrough on how the pieces should fit together. It's pretty simple, but you may need some wire strippers to expose more of the wire to get it seat fully into the connectors. 

1. The short wire of the magnetic switch goes in the "GND" port on Port side A.
2. The long wire of the magnetic switch goes in the "2" port on Port side A.
3. If those wires aren't in those exact spots, the tessel will not work.
4. Insert the USB micro-B cable into the appropriate slot. It is a little stiff the first time you put it in. The tessel can run off USB power when plugged into your computer. This if fine for when you are setting up code on your tessel.
5. When you want your tessel to work in the real world, you'll want to hook up your USB power adapter instead of relying on power from your computer.
Note: the wires from the magnetic switch fit very loosely into the tessel, so you'll need to find a way get them to stay.
 
### 4. Push code to tessel with the NPM package via command line commands



### 5. Install tessel onto a door

### 6. Video Tutorial and Demo of the the system in action

<a href="http://www.youtube.com/watch?feature=player_embedded&v=IHuYJmVRc1I
" target="_blank"><img src="http://img.youtube.com/vi/IHuYJmVRc1I/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

1. 0:00-2:30 shows how to use the website
2. 2:31-3:20 shows how to assemble the tessel
3. 3:21-5:26 shows how to put the code onto the tessel with the command line commands via npm
4. 5:27-6:38 shows a basic demo of the device working
