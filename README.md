time-aware-template
===================

Time Aware is a configurable application template that enables you to display time enabled layers in an ArcGIS web map using a time slider.

[View it live](http://www.arcgis.com/apps/Time/index.html?webmap=8a63712c19a8410082f3dc106118b7d1)
#July 2015 Release Updates
Template was re-worked at this release to have a simpler UI and be more configurable. You can now specify a color scheme, change time options and more. 

#Features

**Time** is a configurable application template that enables you to display time enabled layers in an ArcGIS web map using a time slider. The template can be configured with the following option:

- **Map:** Choose the web map used in the application. 


## Instructions

1. Download and unzip the .zip file or clone the repository.
2. Web-enable the directory.
3. Access the .html page.
4. Start writing your template!

[New to Github? Get started here.](https://github.com/)

## Deploying

1. To deploy this application, download the template from Portal/ArcGIS Online and unzip it.
2. Copy the unzipped folder containing the web app template files, such as index.html, to your web server. You can rename the folder to change the URL through which users will access the application. By default the URL to the app will be `http://<Your Web Server>/<app folder name>/index.html`
3. Change the sharing host, found in the config/defaults.js file of the application, to the sharing URL for ArcGIS Online or Portal. For ArcGIS Online users, keep the default value of www.arcgis.com or specify the name of your organization.
  - ArcGIS Online Example:  `"sharinghost": location.protocol + "//" + “<your organization name>.maps.arcgis.com`
  - Portal Example where `arcgis` is the name of the Web Adaptor: `"sharinghost": location.protocol + "//" + "webadaptor.domain.com/arcgis"`
4. If you are using Portal or a local install of the ArcGIS API for JavaScript, change all references to the ArcGIS API for JavaScript in index.html to refer to your local copy of the API. Search for the references containing `"//js.arcgis.com/3.13"` and replace this portion of the reference with the url to your local install.
  - For example: `"//webadaptor.domain.com/arcgis/jsapi/jsapi"` where `arcgis` is the name of your Web Adaptor.
5. Copy a map or group ID from Portal/ArcGIS Online and replace the default web map ID in the application’s default.js file. You can now run the application on your web server or customize the application further.

**Note:** If your application edits features in a feature service, contains secure services or web maps that aren't shared publicly, or generate requests that exceed 200 characters, you may need to set up and use a proxy page. Common situations where you may exceed the URL length are using complex polygons as input to a task or specifying a spatial reference using well-known text (WKT). For details on installing and configuring a proxy page see [Using the proxy](https://developers.arcgis.com/javascript/jshelp/ags_proxy.html). If you do not have an Internet connection, you will need to access and deploy the ArcGIS API for JavaScript documentation from [developers.arcgis.com](https://developers.arcgis.com/).


#Requirements

- Notepad or HTML editor
- Some background with HTML, CSS and JavaScript
- Experience with the ArcGIS API for JavaScript is helpful. 

#Resources

- [ArcGIS API for JavaScript Resource Center](http://help.arcgis.com/en/webapi/javascript/arcgis/index.html)
- [ArcGIS Online] (http://www.arcgis.com)
- Want to create your own template? View the [Application Boilerplate](https://github.com/Esri/application-boilerplate-js) to get started. 
- [View the Time Aware template on ArcGIS Online] (http://www.arcgis.com/home/item.html?id=24b97891184d4da082ec7d4ab144297e)
#Issues
Found a bug or want to request a new feature? Please let us know by submitting an issue. 

#Contributing
Anyone and everyone is welcome to contribute. 

#Licensing 

Copyright 2012 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's license.txt file.
