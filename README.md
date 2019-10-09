# Application test for the second part of the Technigo frontend boot camp

We're happy that you are applying for the second part of our boot camp. The second part involves a lot of React and Node.js so we would like to check that you are up to speed with more basic HTML, CSS and JavaScript before we offer you a seat. This is so that we all can move forward in the same speed. 

Therefore, we would like to see how you solve this assignment and that you know your way of using git and github. After you have finished the assignment we would like to know a bit more about yourself and why you would like to enter this program in the written application below. 

Fill in this application after you have solved this assignment. 

You last day to submit is on October 23rd. You can expect an answer from us within 5 working days from when you have submitted your assignment. The program starts on November 18th. 

Good luck! 

## Build a Weather Dashboard 

Your task is to build a simple weather dashboard that tells today's weather and temperature using a weather API. Your finished solution should look something along the lines of this:

![Design](https://github.com/Technigo/assignment-weather/blob/master/weather_app.png)

## What we want to see from your solution
* Your usage of HTML and CSS
* Your usage of JavaScript
* The way you are fetching and using the API

## How to complete this assignment

### Get started with the weather API.

[Sign up for a free Open Weather Map account](https://home.openweathermap.org/users/sign_up). Once signed in, go to the "Api Keys" tab and copy the API Key. You can use the API Key in the APPID parameter when making calls to the openweathermap API.

For example, to get the current weather in Stockholm, you can use the url below. Remember to replace "YOUR_API_KEY" with the API key you copied from your dashboard.

http://api.openweathermap.org/data/2.5/weather?q=Stockholm,Sweden&units=metric&APPID=YOUR_API_KEY

The response should look something like this (this has been run through jsonlint.com to add newlines and indentation):

```json

{
	"coord": {
		"lon": 18.06,
		"lat": 59.33
	},
	"weather": [{
		"id": 800,
		"main": "Clear",
		"description": "clear sky",
		"icon": "01d"
	}],
	"base": "stations",
	"main": {
		"temp": 6.47,
		"pressure": 1007,
		"humidity": 56,
		"temp_min": 6,
		"temp_max": 7
	},
	"visibility": 10000,
	"wind": {
		"speed": 3.6,
		"deg": 200
	},
	"clouds": {
		"all": 0
	},
	"dt": 1509709800,
	"sys": {
		"type": 1,
		"id": 5420,
		"message": 0.0024,
		"country": "SE",
		"sunrise": 1509689610,
		"sunset": 1509720490
	},
	"id": 2673730,
	"name": "Stockholm",
	"cod": 200
}
```

As you can see, there's a bunch of useful information in there - including current temperature, windspeed, humidity, etc.

You will need to use the `fetch()` function in JavaScript to load the weather data into your page, and then select the values you want to inject into the DOM from the JSON which comes from the API.

### Present the data on your page

Your task is to present the data: the city name, the temperature (rounded to 1 decimal place), and what type of weather it is (the "description" in the JSON).

Once you get the data onto your page, style your page however you'd like to with CSS, OR add more data to make it even more useful! See suggestions in the stretch goals section.

## How to hand in this assignment. 

To hand in this assignment you need to create your solution and then make sure it's avalible on Github. The link to your repo should be shared with us in the written application form. 

### :books: Reading List

* [MDN Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
* [MDN Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
* [Open Weather API Documentation](https://openweathermap.org/current)
* [.toFixed()](https://www.w3schools.com/jsref/jsref_tofixed.asp)

---

### :sos: How to get help

If you have any questions, feel free to reach out on hello@technigo.io. 
