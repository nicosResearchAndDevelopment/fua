# The Weather Station

## Introduction

The "Weather Station" is the basic example to introduce `fua`s concepts and mechanics. At a first glance it 
behaves as a reflector of well known qualities, like temperature and humidity, etc. and so comes easily like any
other IoT (internet of things) agent and exposed to some services it acts as a "Digital Twin", as a presenter of 
underlying physical truth.

Due to its "unpretentious" nature Weather Station seem to be a good starting point to explain more elaborated concepts
of designing its construction plan, its functions and protecting its information using Access Control mechanisms and 
presenting information in a consumer friendly manner (so the reader of device data - or in the end:
the weather-properties themselves...) 

Weather Station does **NOT** focus on the Service Instance (with given role "provider"), so one Service Consumer
(itself a Service Instance with given role "consumer") can fetch, read information of interest. Service related issues
are presented in gbx ("GAIAboX").

## Weather 

Weather Station makes some assertions about the weather at a very special point in time. This state seems to be an
easy claim. To judge its (The Weather) quality is a total different story. Let's make this assertion:

```pseudocode
weather is nice
```

...to answer this "if it is _really_ nice", we have to make a deep dive to a more generic concept of _complex contexts_.
So, "Weather" is the starting example to get in touch with those.

---
