# Engineering for the Stratosphere

[Video](https://www.youtube.com/watch?v=8IwazMmHWvc)

## Project Loon
The question they try to answer: Could we get EVERYONE connected, across the globe, no exceptions?

How Loon works:
 - Mobile connects directly to the balllon
 - The fleet of balloons adjusts as a network to ensure continuous coverage
 - Uses wind currents on stratosphere to navigate precisely at high altitudes

Balloons go up to 25km in the sky. Move at +300 km/h.

They built a Mission Control system to monitor the balloons. Not a massive control center, it runs on a mobile!
Provides real-time monitoring and tracking

Diagnosing the ballon's health is tricky: combination of sensors (GPS, pressure) and algorithmic analysis. Temperature measuring is hard, so they measure sun radiation, and feed it to a balloon temperature model to determine temperature.

With temperature, they can estimate balloon lifetime (depends on temperature and amount of gas in balloon).

Power predictions: they use solar on day + batteries for night, but predicting power consumption is hard. Temperature affects battery behavior a lot. They've a custom charge estimator based on their observations.

Wind data and altitude models to create simulated balloon trajectory.

http://google.com/loon