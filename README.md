# FlipTrip
##### Uber for Dumb Phones

FlipTrip gives Uber access to those without smartphones. Using FlipTrip's simple SMS interface, now *any* phone can request an Uber!

Made at PennAppsXII

![screen shot](https://raw.githubusercontent.com/3RPM/FlipTrip/master/screen_shot.png)

## Installation

* Clone the repo and run `npm install`
* Copy `config.sample.json` to `config.json` and input the appropriate values
	* For the Uber API, you will have to request permission to use the `request` endpoint in order to order Ubers
* In your Twilio control panel, configure a webhook to point a POST request to `http://your.url/twilio_webhook`
* Run `node app.js` to start your server

## Usage

* Navigate to `http://your.url/verify`, and grant Uber permission
* Text the number you configured `hmu` or `send me an uber`
* Text in your location
* Text in your destination
* Await your Uber!
* Text `jk` to cancel your Uber
* Text `?` for help

**Note:** you don't actually need a location and destination "address". Anything that would work if you typed it into Google Maps would work, like just `Wells Fargo Center, PA` or `University of Pennsylvania`.


## WARNING

This is in beta. Use at your own risk.


## Todo

* Clean code
* Give updates via text about driver's location