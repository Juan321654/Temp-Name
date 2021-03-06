# The Weather Teller

## Deployed Site
https://theweatherteller.netlify.app/


## Project Description

The Weather Teller its a place where you can find the current weather in your area or other cities. 
do you want to go out to the beach? Maybe go on a picnic? This app will let you know how windy, cloudy, rainy, or humid it is outside so you can plan accordingly.

## API and Data Sample

https://openweathermap.org/current

Sample JSON:
```json
{
    "coord": {
        "lon": -73.92,
        "lat": 40.83
    },
    "weather": [
        {
            "id": 803,
            "main": "Clouds",
            "description": "broken clouds",
            "icon": "04d"
        }
    ],
    "base": "stations",
    "main": {
        "temp": 301.4,
        "feels_like": 299.47,
        "temp_min": 300.37,
        "temp_max": 302.59,
        "pressure": 1016,
        "humidity": 48
    },
    "visibility": 10000,
    "wind": {
        "speed": 5.7,
        "deg": 50
    },
```

## Wireframes

https://wireframe.cc/DBy7pV
 

#### MVP 

- choose a city
- choose between Fahrenheit and Celsius
- display weather conditions such as humidy, cloudy etc.

#### PostMVP  

- make the background change to warm or cool colors depending on the temp
- make transition effect when clicking F to C
- make a transition to the background when changing colors
- make text color change according to temp
- make city, icon, temp, description, conditions fade in when called.

## Project Schedule

|  Day | Deliverable | Status
|---|---| ---|
|August 14-16| Prompt / Wireframes / Priority Matrix / Timeframes | Complete
|August 17| Project Approval | Complete
|August 18| Core Application Structure (HTML, CSS, etc.) | Complete
|August 19| Initial Clickable Model  | Complete
|August 20| MVP | Complete
|August 21| Presentations | Incomplete

## Priority Matrix

[![Matrix1.png](https://i.postimg.cc/gjr4NpKj/Matrix1.png)](https://postimg.cc/T5Mr3ZFv)

## Timeframes


| Component | Priority | Estimated Time | Time Invested | Actual Time |
| --- | :---: |  :---: | :---: | :---: |
| HTML structure | L | 2 hrs|  | 1hr |
| Working with API | H | 3hrs|  | 6hr |
| Basic CSS | L | 3hrs|  | 5hr |
| changing C to F | H | 2 hr|  | 5hr |
| displaying conditions | H | 3 hrs|  | 2hr |
| displaying city | H | 3 hrs|  | 3hr |
| displaying weather icons | H | 3 hrs|  | 2hr |
| changing text color/icons | H | 3 hrs|  | 1hr |
| Total | H | 22 hrs|  | 25hrs |
## Code Snippet

making this function took me hours but it forced me to understand better how to talk to the computer. 

```
function switchFtoC (target) {
  celsiusButton.addEventListener('click', () => {
    tempValue.innerHTML = Math.round((parseInt(target) - 32) * 5/9) + '\xB0C';
  })
}
```

## Change Log
for the post MVP I'm not doing the weather description fade in because the page will look too empty without them displaying right away and the background i chose macthes every icon for the wather, and i like it like this better than changing the background (not the icon) color depending on temperature.
