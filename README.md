# One to One Video Calling Application using Vue.js (JS Framework) and Airtel IQ Toolkit for Web

This is a sample one to one video calling client application in VueJS that allows developers to implement video calling capabilities in their websites. The application runs on the web browsers (referred as client end point) and utilizes Airtel IQ Web SDK to conduct an RTC session with its peers through Airtel IQ Video Services. 

The client application performs the following tasks to facilitate an RTC session: 

* Get token from the application server 

* Connect to the room using the token 

* Publish audio/video streams in the room 

* Subscribe to remote audio/video streams in the room 

* Listen to any session related events

This sample client application also demonstrates the following features:

* Mute/Unmute video 

* Mute/Unmute audio 

* Disconnect



## 1 Get Started

### 1.1 Pre-Requisites

### 1.1.1 Authorization Credentials

* [Access Airtel Video IQ Portal](https://cpaasportal.videoiq.airtel.in/)  
* Create your Project
* Get the App ID and App Key generated against the Project


### 1.1.2 Requirement

* Check your [browser compatibility with Airtel IQ](https://www.videoiq.airtel.in/developer/video/browser-compatibility-of-airtel-iq-video/) 
* Download latest copy of [Web SDK (EnxRtc.js)](https://www.videoiq.airtel.in/developer/wp-content/uploads/EnxRtc.js.v1.0.0.zip)  and replace public/EnxRtc.js 


### 1.1.3 Clone

Clone this ``` git clone https://github.com/airteliq/Airtel-IQ-One-to-One-Video-Chat-Sample-Web-Application-Vuejs-Client.git ```  


### 1.1.4 Sample Application Server

While this GitHub repository provides sample client code, you require an application server to provision video room on Airtel IQ server.**Clone or download repository of your choice and configure the server as per the instructions given in the respective README document of the server repository chosen.** Use any of the Repository listed below to setup your application server: 

* [Nodejs](https://github.com/airteliq/Airtel-IQ-One-to-One-Video-Chat-Sample-Web-Application-NodeJs-Server)

* [C#](https://github.com/airteliq/Airtel-IQ-One-to-One-Video-Chat-Sample-Web-Application-C-Sharp-Server)

To directly try the sample code without having to configure an application server, you can also use the Airtel IQ test server as explained in section 2. However, it is recommended to configure your own application server to build a video calling web app. 

#### 1.1.5 Merge the client and server repositories
Once the ReactJs client side repository is cloned inside the server repository, follow the points listed below:

* ``` cd Airtel-IQ-One-to-One-Video-Chat-Sample-Web-Application-Vuejs-Client ```

* To install all project modules.Run ``` npm install ```


### 1.2 Build Application  

Run `npm start` 


### 1.3 Test 

* Open the web browser and go to https://your-domain-name:8080/ to load the application.  
* If you don't have a Room ID, then create by clicking on the “Create Room” button. The Room ID will get prefilled in the form. 
* Save the Room ID and share it with others along with the URL to join the Same Room.  
* Enter your Name and choose your role, either as a Moderator or a Participant 
* Allow access to the microphone when prompted. 
* You are now in a video call with others, who have joined the same room. 

Note: This sample application creates a virtual room with limited Participants and 1 Moderator for demonstration purposes. 


## 2. Pre-Configured Testing Environment

As mentioned in section 1.1.4 above, you have an option to run your client application on [**Airtel IQ pre-configured environment**](https://try.videoiq.airtel.in/) instead of setting up your own application server.  

This allows you to quickly test the performance of Airtel IQ audio calls before getting into the development of your application.  

As the Airtel IQ test server has been configured for demonstration purpose only, it only allows to: 

* Conduct a single session with a duration lesser than 10 minutes. 
* Host a multiparty call with less than 3 participants. 

Refer to the [**Demo App Server**](https://www.videoiq.airtel.in/developer/video/sample-code/#demo-app-server) for more information.   

Once you have successfully tested your application on the test server, you can set up your application server as explained in section 1.1.4 above. 



## 3. Learn more about Client API

The client APIs are called from the Airtel IQ Web SDK (EnxRtc.js) which runs on the client browser. The client APIs are used to communicate with the Airtel IQ video services and monitor the client-side state of the RTC session.  

The client APIs are typically used to: 

* Connect to the desired room using the token received from the application server 
* Manage local audio and video 
* Handle room and stream related events initiated by the user 

The client APIs handle four major entities: 

* **Airtel IQ Room:** It handles room/session related events like connection, local stream publication, and remote stream subscription. 
* **Airtel IQ Stream:** It identifies audio/video/data stream published by the user. 
* **Events:** It represents the events related to the room and the stream. 
* **Player:** It represents the customizable UI element used to render the audio/video stream in the DOM. 

In addition to the features demonstrated in this sample program, the SDK has many helpful APIs available for the developers to utilize like: 

* File sharing 
* Streaming 
* Annotation 
* Canvas 

And many more such exciting features. 

Read [**Web Toolkit Documentation**](https://www.videoiq.airtel.in/developer/video-api/client-api/web-toolkit/)  for more details.  

[**Download Web Toolkit**](https://www.videoiq.airtel.in/developer/wp-content/uploads/EnxRtc.js.v1.0.0.zip) to get the latest version of Web SDK. 



## 4. Support

Airtel IQ provides a library of Documentations, How-to Guides, and Sample Codes to help software developers, interested in embedding RTC in their applications. 

Refer to the [**Complete Developer’s Guide**](https://www.videoiq.airtel.in/developer/video-api/client-api/) for more details. 

You may also write to us for additional support at support@videoiq.airtel.in. 
