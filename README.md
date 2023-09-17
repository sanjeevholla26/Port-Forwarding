# Port-Forwarding
<br>

## Practicle implementation and theoretical explanation of PORT FORWARDING

#### What is Port Forwarding?
It is just forwarding the port of your router so that any request comming to that router through that port will be forwarded to a particular device connected to its network.
* How internet works is, when ever we want to access something via internet for example a website, then we need to send a request to the server(which is a computer itself) in which the website is hosted.
* When we send a request from our device, the request will first reach our router and from our router it gets transfered into different routers and at last it reaches the destination computer.
* So requests will be in the form of packets.
* When ever a packet reaches a router or any device it passes through a particular port.
* So when we access a website, we will not just send a request to a device where it is hosted but also to a particular port of that device in order to get the website.

### Turn your computer into a Server

If we want to host a website on our device only and make it accessible to the whole world then you might need to do ***PORT FORWARDING***
* You need specify that whenever a request is comming to a particular port of the router then it should be redirected to your device.
* So by doing so, you can host your website on the localhost(means on your IP address) at a particular port say 10000. Now do port forwarding such that when ever a router receives a request to a particular port lets say 8000, it should redirect that request to the port 10000 of your device.
* So when somebody wants to access the website which you are running on the localhost, then they should send the request to the 8000th port of your router which automaticaly forwards it to your device's 10000th port where your website is running.
Like this your computer can become a server.
   
