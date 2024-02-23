# ha_lowestchargeprice
This uses the energidataservice to find hour with the lowest price

This will find the lowest price, to use to find out when to charge your EV.
You can define fx 5 hours. I will then return the hour for when it's cheapest to charge your EV for 5 hours.

- Create a Template helper entity in Home assistant
- Choose 'Template a sensor'
- Give it a name
  unit of measure = h
  Device class = Duration
- Add the template
  Change the timespanInHours and beforeHour int the template to fit your needs

timespanInHours: defines how many consequently hours the price spans
beforeHour: defines the hour, when the charge should be finished (ex: 7 if the charge should be finished before 7:00)
