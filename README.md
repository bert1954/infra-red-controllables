The Infra Red Controllables Repository
=======================

Welcome to the Infra Red Controllables Repository. 
This repository will allow you to add devices which can be controlled by the WunderBar IR sensor. 

We've added the first device - a Led Strip.

## Adding your device to the Repository

Dvices are defined in JSON files which contain
the device's details as well as the commands it is capable of receiving.

In order to define your device simply follow the Led Strip example: 

### 1. Start by adding some information about the device: 

    "name":"LED Strip",
    "meta":{
      "productName":"LED strip",
      "manufacture": "LED strip  inc.",
      "website": "http://www.led.strip.com",
      "image":"http://www.led.strip.com/image."
    },
  
 The `name` is the only mandatory attribute in this section.
 All information within `meta` is optional.
 
### 2. Continue by adding an array of the commands the device is capable of receving.

    "commands":[
    {
      "title":"ON",
      "command":13
    },        

    {
      "title":"OFF",
      "command":31
    },
    {
      "title":"BRIGHT+",
      "command":9
    },
    ...
  ]
  
