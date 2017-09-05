<h1 align="center">
  <br>
  P.O.L.L.I.
  <br>
  Program Operated Load Lifting Instrument
  <br>
  <img src="http://www.robotshop.com/media/files/images2/lynxmotion-al5d-4dof-robotic-arm-ssc-32u-combo-kit-no-software-1-large.jpg" alt="AL5D Lynxmotion Robotic Arm" width="700">
  <br>
</h1>

## Key Features
* Control AL5D Lynxmotion Robotic Arm by hand gestures via LeapMotion controller
* Control AL5D Lynxmotion Robotic Arm by web-based user-interface controls
* Analytics for tracking mechanical functions

## Technologies Used
- [jQuery](http://www.w3schools.com/jquery/jquery_ref_ajax.asp) - jQuery simplifies HTML document traversing, event handling, animating, and Ajax interactions for rapid web development.
- [Node.js - NPM](https://www.w3schools.com/nodejs/nodejs_npm.asp) - NPM is the package manager for JavaScript and the world’s largest software registry. Discover packages of reusable code — and assemble them in powerful new ways.
- [Socket.io](https://socket.io/) - Socket.IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers.
- [Johnny-Five](http://johnny-five.io/) - Johnny-Five is an Open Source, Firmata Protocol based, IoT and Robotics programming framework, designed for anyone who wants to get started with JavaScript-powered robotics.
- [Firmata](https://github.com/firmata/protocol) - Firmata is a protocol for communicating with microcontrollers from software on a computer (or smartphone/tablet, etc).
- [Express](https://expressjs.com/) - Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

## Setup and Install

Pin Layout:
* Pin 13 - Led
* Pin 12 - Wrist Servo
* Pin 10 - Elbow Servo
* Pin 9 - Shoulder Servo
* Pin 8 - Piezo Buzzer
* Pin 6 - Claw Servo
* Pin 3 - Base Servo

To clone and run this application, you'll need [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

## To run LeapMotion gesture control

```bash
# Clone this repository
$ git clone https://github.com/irishdowd10/P.O.L.L.I

# Go into the repository
$ cd P.O.L.L.I

# Install dependencies
$ npm install

# Run the app
$ node robotarm.js
```

## To run web-based user-interface controls

```bash
# Clone this repository
$ git clone https://github.com/irishdowd10/P.O.L.L.I

# Go into the repository
$ cd P.O.L.L.I

# Install dependencies
$ npm install

# Run the app
$ npm start

# Open localhost
Open web browser and go to http://localhost:4200
```

## Troubleshooting
Possible errors may occur when running npm start from terminal:

```bash
Error: Cannot find module './mixins/collection'
    at Function.Module._resolveFilename (module.js:485:15)
    at Function.Module._load (module.js:437:25)
    at Module.require (module.js:513:17)
    at require (internal/module.js:11:18)
    at Object.<anonymous> (/Users/dlopez6877/Desktop/P.O.L.L.I/node_modules/johnny-five/lib/board.js:17:18)
    at Module._compile (module.js:569:30)
    at Object.Module._extensions..js (module.js:580:10)
    at Module.load (module.js:503:32)
    at tryModuleLoad (module.js:466:12)
    at Function.Module._load (module.js:458:3)
```
to resolve this issue:
* open package.json and remove johnny-five from dependencies.
* from terminal run: $npm install johnny-five --save

```bash
Error: Cannot find module 'socket.io'
    at Function.Module._resolveFilename (module.js:485:15)
    at Function.Module._load (module.js:437:25)
    at Module.require (module.js:513:17)
    at require (internal/module.js:11:18)
    at Object.<anonymous> (/Users/dlopez6877/Desktop/P.O.L.L.I/webtest.js:7:8)
    at Module._compile (module.js:569:30)
    at Object.Module._extensions..js (module.js:580:10)
    at Module.load (module.js:503:32)
    at tryModuleLoad (module.js:466:12)
    at Function.Module._load (module.js:458:3)
```
to resolve this issue:
* open package.json and remove socket.io from dependencies. (don't forget the comma after johnny-five)
* from terminal run: $npm install socket-io --save

### License

**P.O.L.L.I** © 2017, Daniel Lopez, Isabella Abatgis, Pete Lazuran, John Dowd. Released under the [MIT License].
> GitHub [@Sigtaba](https://github.com/Sigtaba) &nbsp;&middot;&nbsp;
> GitHub [@dlopez6877](https://github.com/dlopez6877) &nbsp;&middot;&nbsp;
> GitHub [@Naruzal](https://github.com/NaruzaL) &nbsp;&middot;&nbsp;
> GitHub [@irishdowd10](https://github.com/irishdowd10) &nbsp;&middot;&nbsp;
