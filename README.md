# Hail warner for Home Assistant - based on VFK API (Switzerland only!)
easy to use API for hail warning in Switzerland (only in Switzerland) from Vereinigung Kantonaler Feuerversicherungen (VKF)
 

## Get access to the API
Follow the process here: 
https://www.hagelschutz-einfach-automatisch.ch/eigentuemer-verwaltungen/produkt/ich-habe-interesse.html


## Sensor 
the hail.yaml needs to be in the HA directroy

> Replace XXXX and YYYY with the information you got from VFK


## Import the hail.yaml in the configuration.yaml

```
#####Hail Status VFK####
rest: !include hail.yaml
```

## Automation
in my case, i use a shelly - use what ever fits for your purpose. Important are the triggers, the sensor goes to 1 if hail is forcasted. the test alert sets the value of 2. 
