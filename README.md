# Cordova Check Installed Service Plugin

Plugin to check from where app is installed from like Play Store, Baidu , Amazon etc.


## Using

In your cordova project folder:

    $ cordova plugin add https://github.com/Anand1907/cordova-plugin-check-services.git


Then the variable 'CheckServices' will be available after `deviceready` fires.

CheckServices.check(successCheckServices, failureCheckServices);


successCheckServices contains an type attribute from which application can check the installer name.


function successCheckServices(message) {

    console.log(message.type);      // This helps you to get the installer package ir-respective to store.

}

function failureCheckServices(message) {

    console.log(message.error);     // Error string from Stack Trace

}
