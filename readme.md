# We-connect

It is a Webrtc. Check report file to know more

## Installation

### Install Node.js in your system and set it to path

Now open your terminal window and set its directory to the src folder or if using VS code then open that folder with VS code and then open VS code terminal and then type these codes one by one.

```
npm install -g nodemon

nodemon server.js
```

## Usage

Now open your browser and in the url box type:
```
localhost:8000
```

## If trying to deploy

### In server.js change
```
server.listen(8000);
```
to
```
server.listen(process.env.PORT||3030);
```
### In script.js change
```
var peer = new Peer(undefined,{
    path: '/peerjs',
    host: '/',
    port: '8000',
}); 
```
to 

```
var peer = new Peer(undefined,{
    path: '/peerjs',
    host: '/',
    port: '443',
}); 
```
