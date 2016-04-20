# Cordova Google Play Services Check

Simple cordova plugin for checking that the google play services are installed, updated and enabled. 

## Using

In your cordova project folder:

    $ cordova plugin add cordova-plugin-googleplayservices-check


Then the variable 'GooglePlayServicesCheck' will be available after `deviceready` fires.

```js
	document.addEventListener('deviceready', function () {
	
		var success = function(response) {
			// response.isGooglePlayServicesAvailable is a boolean value
			response.isGooglePlayServicesAvailable;
		} 

		var failure = function(response) {
			response.isGooglePlayServicesAvailable;
		}

		GooglePlayServicesCheck.check(success, failure);
	})
```

