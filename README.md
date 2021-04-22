# Let's containerize the Node.js project!

Our goal is to containerize this application.

## Exercise: Dockerfile

Our goal is to write a Dockerfile for the Node.js container.

First, `git clone` this repository. 

This is a demonstration Nodejs web server. 

To install the dependences run:
```
yarn install --production
```

To run the node server:
```
node src/index.js
```

Important: You should use node version: `12.22.1`

The port exported by the application is 3000

## Test the application

After you have created the Dockerfile, run the follow commands to test it:
```
~$ docker build -t node-demo .
~$ docker run -p 3000:3000 node-demo
```

Go to http://localhost:3000
