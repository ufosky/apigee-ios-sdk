#Apigee iOS SDK Sample Apps

The sample apps in this directory are intended to show basic usage of some of the major features of App Services using the Apigee iOS SDK. By default, all of the sample apps are set up to use the unsecured 'sandbox' application that was created for you when you created your Apigee account.

##Included Samples Apps

* **assets** - An app that shows you how to attach image assets to entities and also shows how they can be downloaded and used.
* **books** - A 'list' app that lets the user create, retrieve and perform geolocation queries on a list of books. This sample also makes use of jQuery and jQuery mobile.
* **collections** - An app that shows you how to perform basic CRUD operations on collections in your account.
* **events** - An app written in Swift that acts as an EventBrite clone.  This shows you how to integrate the SDK using the Swift programming language and some of the general functionality. 
* **entities** - An app that shows you how to perform basic CRUD operations on entities in your account.
* **geolocation** - An app that shows you how to creates entities with location data, and perform geolocation queries to retrieve them.
* **messagee** - A Twitter-like app that uses data store, social and user management features.
* **monitoringSample** - An app that lets you test the App Monitoring feature by sending logging, crash and error reports to your account.
* **oauth2** - An app that demonstrates the use of OAuth 2 access token retrieving, using and storing with the Apigee SDK.
* **push** - An app that sends push notifications to mobile devices using APNS or GCM.
* **usersAndGroups** - An app that shows you how to create and manage user and group entities.

##Running the sample apps

To run the sample apps, simply open the .xcodeproj file in Xcode, then run the app.

Before you do, however, you will need to build the framework by run this command from the `/source` directory of your repository.

    ```bash
    ./Scripts/framework.sh
    ```

Some of the apps also require you to provide your organization name by updating the call to ApigeeClient in the app's source. Near the top of the code in each app, you should see something similar to this:

	```obj-c
    NSString * orgName = @"yourorgname"; //Your Apigee.com username
    NSString * appName = @"sandbox"; //Your App Services app name
    ```

Simply change the value of the orgName property to your Apigee organization name.