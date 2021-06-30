### Simple TCP Load Balancer

#### Technologies used:
1. HAProxy
2. Node.JS application servers

#### Commands to run
```
port=4444 nodemon appserver.js
port=5555 nodemon appserver.js
haproxy -f tcp.cfg
```
```Hit localhost:8080 on browser``` <br><p>
(Add as many ports to tcp.cfg as desired to create more app servers to be load balanced.)

<i>That's all it takes to create a Layer 4 Load Balancer!</i>