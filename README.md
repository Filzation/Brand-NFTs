# Filza's WebAR Starter Kit
This is a customized kit for creating WebAR experiences.

You can find additional notes of each step in the individual files.

---

&nbsp;
> **How to run code via HTTPS connection**

### *1) With NPM serve to host (Preferred)*

``` bash
# Install serve globally (once)
npm install -g serve

# Install ngrok 
npm install ngrok

# Specify the port to use 
serve -p 8080

# Pass local server to ngrok (you might need to open another local terminal)
ngrok http 8080
 
# Test the HTTPS connection on mobile
- Copy the HTTPS url on the 2nd line of the Forwarding
- For eg, https://e1c6-103-252-201-56.ngrok.io
- Type the url on your phone and you should have access to the experience
   
```
---
&nbsp;

### *2) With Web Server for Chrome Setup*
Install [WebServerforChrome](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en)
``` bash
# Launch the app
- Check "accessible on local network" and "Also on internet" (maybe).
- Restart the application after. 

# Choose folder
- Navigate to where your core folder for the project is in.
- For eg, the core folder for this file is "final" as it contains our css, html  & js files.

# Click on the 2nd Web Server url
- A window will pop up showing your UI on your browser.
- You can test/ debug if you need if you have the WebXR API Emulator.

# To test on your mobile without using a connected cable from your PC 
- Create an account and download and do the necessary setup for the program.
- In your command line, write and enter this code: ngrok http 127.0.0.1:8080 -host-header="127.0.0.1:8080"
  Make sure to replace the url with the one you have and remove "http" and "/"  
  
  # Test the HTTPS connection on mobile
- Copy the HTTPS url on the 2nd line of the Forwarding
- For eg, https://e1c6-103-252-201-56.ngrok.io
- Type the url on your phone and you should have access to the experience
    

```
---
&nbsp;




### *2) Without Web Server for Chrome Setup*
Download [Node.js](https://nodejs.org/en/download/).

- Run the following commands:

``` bash
# Install dependencies (only the first time)
npm install

# Run the local server at localhost:8080
npm run dev

# Build for production in the dist/ directory
npm run build

# Install and run ngrok to get HTTPS connection
- npm install ngrok
- ngrok http 8080
```

- If needed, do the following:
``` bash
# Install Webpack Latest Version
npm install webpack@latest 

# Update Html Webpack Plugin
npm i --save-dev html-webpack-plugin

# Install Three.js modules
npm install --save three

# Install Vue.js
npm install vue
```

## Misc

[Webpack v4 to v5](https://webpack.js.org/migrate/5/)

[Html Webpack Plugin](https://www.npmjs.com/package/html-webpack-plugin)

[Three.js](https://threejs.org/docs/index.html#manual/en/introduction/Installation)

To build UI -
[Vue.js](https://vuejs.org/v2/guide/installation.html)

To run localhost to web - [Ngrok](https://stackoverflow.com/questions/55014750/why-ngrok-access-encounter-error-502-bad-gateway)




