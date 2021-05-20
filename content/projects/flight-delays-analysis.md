---
title: "Flight delays analysis"
date: 2020-06-03
menu:
  sidebar:
    name: Flight delays analysis
    identifier: flight-delays-analysis
    weight: 8
---
## 1. Introduction
Have you ever been stuck in an airport because your flight was delayed or cancelled and wondered if you could have predicted it if you'd had more data? This is the goal of this project. 

Using the 2004 US flights, I tried to determine if there was a specific time were flights had more delays. Since there was more then 7 million flights, I had to use PySpark with a map reduce. I was able to determine the mean delays by hour, day of the week and month.   

## 2. Delay by hour
Most delays occur at the end of the day, which is not surprising since there is an accumulation of all the delays of the day. So it's better to travel early in the morning.
{{<img src="https://user-images.githubusercontent.com/47567574/119043589-7d777080-b9b9-11eb-8e17-09136d4a36c8.png" align="center" caption="Delay by hour">}}

## 3. Delay by day of the week
It looks like there are less delays on tuesday, wednesday and on the weekend, even if the difference is not that important. 
{{<img src="https://user-images.githubusercontent.com/47567574/119043658-8ff1aa00-b9b9-11eb-86a8-2e2743bf8caa.png" align="center" caption="Delay by day of the week">}}

## 4. Delay by month
Most delays occur during the summer and at the end of the year. That's when most people go on holidays. 
{{<img src="https://user-images.githubusercontent.com/47567574/119043723-a7309780-b9b9-11eb-91ab-56376acc2e32.png" align="center" caption="Delay by month">}}

## 5. Conclusion
If you hate waiting in the airport, you should travel on an early tuesday in September. 
