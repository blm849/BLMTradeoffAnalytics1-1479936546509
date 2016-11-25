# BLMTradeoffAnalytics1


This is a simple example of how to work with IBM Watson's Tradeoff Analytics using node.js and their API.
  
It uses the JSON input provided in <a href="https://www.ibm.com/watson/developercloud/doc/tradeoff-analytics/tutorial.shtml">this tutorial</a>.
  
Since there was only a tutorial using cURL but no node.js tutorial, I took the tutorial material for cURL to write this simple node.js application.

The application is very simple. If you go to https://blmtradeoffanalytics.mybluemix.net you will see an online form you can fill in. The application knows about seven different mobile phones, and based on what you enter, it will use Watson's Tradeoff Analytics service to determine which of the seven are good for you.  

That's it!
   
For more information on the API, click <a href="https://www.ibm.com/watson/developercloud/doc/tradeoff-analytics/">here</a>.

## About the application

The application is a simple node.js application that has integration to the Watson Tradeoff Analytics service.  It can run on IBM's Bluemix service or it can run locally. 

The application uses a number of node.js packages, such as express, ejs and watson-developer-cloud, among others. The static content (e.g. about.html and the CSS file(s)) are found in the **public** directory. The EJS files are located in the **views** directory.

The main application file is app.js. Another key file is config.js. If you use this repo to build your own working application, you will need to make a config.js file from the provided file "config.js.to_be_configured". This file has your Tradeoff Analytics username and password.

## Run the application locally
If you want to run this application locally

1. [Learn about Tradeoff Analytics]
2. Download and extract the code into a directory.
3. Get a Bluemix account if you don't have one already.
4. Get your Bluemix credentials with regards to Tradeoff Analytics. For more information on that, see [getting started].
5. Get your Tradeoff Analytics username and password and create a config.js file with this information.  
6. [Install Node.js]
4. cd into the directory you downloaded the code
5. Run `npm install` to install the app's dependencies
5. Run `npm start` to start the app
6. Access the running app in a browser at http://localhost:6001
7. Create a Bluemix app and upload your application to Bluemix. [See here for more on this].

[Learn about Tradeoff Analytics]:https://www.ibm.com/watson/developercloud/doc/tradeoff-analytics/index.shtml
[Install Node.js]: https://nodejs.org/en/download/
[getting started]:https://www.ibm.com/watson/developercloud/doc/getting_started/gs-credentials.shtml#getCreds
[See here for more on this]:https://console.ng.bluemix.net/catalog/starters/sdk-for-nodejs/?taxonomyNavigation=applications
