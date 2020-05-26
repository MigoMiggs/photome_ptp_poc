# Photome (peer to peer) poc

## Setup 

1. Install node js 
https://nodejs.org/en/

2. Install peer-js server
https://github.com/peers/peerjs-server

3. Start peer-js server 
peerjs --port 9000 --key peerjs --path /myapp

4. Start the node app that is part of this repo (this is for serving static files) - this will run on port 3000
node app.js

## Run the code

Open a chrome window/tab and navigate to:
http://127.0.0.1:3000/send.html

Open another windopw/tab and navigate to:
http://127.0.0.1:3000/receive.html

## Run the whole experience

### Video stream flow

From Send:
* Click "Get Camera Stream," it wlil ask you to allow chrome to access your camera, go ahead

From Receive: 
* Click the gray box, don't expect anything... it's a weird glitch at the moment but has to be interacted with before it shows video

From Send:
* Click "Call peer with stream," eventually video should start streaming on receive.html

### Shutter click flow

From Semd:
* Click connect
* Type some text inside message and click "send"
* Verify that you get the message inside receive.html

From Receive:
* Type "click" within message window, and click "send"
* You should see a snap taken and placed in the bottom of send.html




