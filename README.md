# Caffeine Monitor

During the Build Conference 2010, a caffeine monitor was produced as a collaborative effort between the Campaign Monitor (http://www.campaignmonitor.com) folks, Nicholas Felton (http://feltron.com/) and Go Free Range (http://gofreerange.com).

Their system used a smart phone app that required a human to monitor how many cups of coffee were consumed. The results that were collected from the app were collated, and displayed on the Caffeine Monitor dashboard.

Around the same time, my then employer brought in "Bean to Cup" coffee machines, and a good 90% of the workforce was wired up on caffeine to the detriment of their health (headaches, sleepless nights, stomach upsets and nausea to name a few), so I decided to monitor caffeine consumption and asked Nicholas if i could use his dashboard design, and he agreed (thanks!).
My system differed in that is communicated directly with the coffee machine (in fact the coffee machine was able to tell us when it would run out of beans).
## What is it?
Caffeine monitor is fun way to display how much caffeine has been consumed by a given audience.
The system connects to caffeine vending machines (e.g. automated coffee vending machines) via the diagnostic RS232 interface.
Almost all of these types of machines offer some sort of indication of what is being dispensed, although there is no standardised protocol. Your millage may vary.

All the systems emit some sort of ASCII message. The most basic systems will issue a statement to that fact that a drink has been dispensed by issuing the price, followed by a carriage return and line feed.
: 0.00 <CR><LF>
Other systems will emit messages all day long, giving current stock levels, and various operating parameters (temperature of boiler, pressure of mains water etc.).

In each case, the messages have to continually monitored, parsed and the events that we are interested (the vending of a caffeinated drink) captured for display on the caffeine monitor.


## What’s in the repo?
Right now its little more than a mock of the dashboard HTML, and styling.
