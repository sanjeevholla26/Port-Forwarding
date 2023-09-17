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

### How to do PORT FORWARDING

* For this we need to get the router web interface. So run the following command in the terminal(Linux).
  <br>
  
        ip route | grep default
  
  <br>
  Enter the IP address which you will get after running the above command in the browser to get the web interface of the router.
  
![image](https://github.com/sanjeevholla26/Port-Forwarding/assets/104841119/9f028cdb-2f2c-49c8-9eee-96b3f9b74e6a)

* Now you need to enter the default usename and password for your router. (Remember its not the same as your username and password of your wifi. Search in google to get them).
  <br>

  ![image](https://github.com/sanjeevholla26/Port-Forwarding/assets/104841119/9e0cd180-4256-4f69-a540-9a75eeaa238d)

* Now go to Application and there select Port forwarding

  ![image](https://github.com/sanjeevholla26/Port-Forwarding/assets/104841119/5644ce31-4f40-4fce-9be7-c2bdd2ee7a95)

* Now here you need to give the details in order to do the PORT FORWARDING.
* ***WAN-Port*** - The port of the router which will be listening for the request.
* ***LAN-Port*** - The port of the device to which the router will forward the request to.
* ***Internal client*** - To which device lan port the request should be forwarded to.



   
