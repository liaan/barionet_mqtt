# bartionet_mqtt
Library code to run mqtt on Barionet.

This still very much alpha maaybe beta version. It works, but in controlled enviroment.

* limit of 126 topic and data length (should never be that in proper configured mqtt) .
* QOS 0 only, might improve this if there ever need
*

# Usage
* Sending publish
```

    MqTopic$ = "barionet/alarmscene/"+str$(subgroup)+"/value"
    MqMessage$ = str$(group)
    MqRetain = 1 ''Enable Retain flag
    gosub 5260
```
* Subscribe
```
	MqTopic$ = "barionet/scene/+/set"
	gosub 5360
```



