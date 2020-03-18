# Dashboard


## About Dashboard
It's a pretty simple dashboard, which was initially going to be used on a Raspberry Pi for a wall mounted screen. I decided to put it up on here incase someone wanted to use it.

Currently it gets the current time and date from the system, pulls the current weather from Cardiff, UK using [Open Weather Map](https://openweathermap.org/) and the top 10 headlines from the BBC using [NewsAPI](https://newsapi.org)


## Customising Dashboard for use
There are currently four main things to add to get this working, which is an API Key for both Open Weather Map and News API, which are both free, but limited, although this shouldn't be a problem at default update settings.

You need to sign up for [Open Weather Map's API](https://openweathermap.org/api) here, and then [News API's API here](https://newsapi.org/register).
The API Key can be entered into the apiKey const under the ServiceWeather and ServiceNews 

The third setting to update is the Weather's location, which at default is set to London, UK and can be changed to any City ID using [Open Weather Map's City ID list](http://bulk.openweathermap.org/sample/city.list.json.gz). This is set by the "location" setting, in the options variable under the ServiceWeather function.

The forth and final setting to change, if you want to, is the news source from it's default, which is BBC News, a list of sources can be found [on NewsAPI's website](https://newsapi.org/)

After setting these, the dashboard should work! Congratulations! Da Iawn!

## Screen sizing
Currently, if the screen is less than 300 pixels high or less than 540 pixels wide, the news will not appear, as it would take up too much screen size, this means the date, time and weather will fill the screen, which might be ideal for a portable screen.