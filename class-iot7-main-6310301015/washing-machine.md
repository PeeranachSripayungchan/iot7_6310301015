![Washing Machine](pictures/iot-machine.png)

## Get hardware level operations e.g. wash_count
```
Topic: v1cdti/hw/get/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "wash_count",
    "value"     : "114"
}
```

## Get firmware version
```
Topic: v1cdti/hw/get/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "firmware_version",
    "value"     : "17"
}
```

## Get manufacture id and geo-location or location placement
```
Topic: v1cdti/hw/get/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "manufacture_id",
    "value"     : "17"
}

Topic: v1cdti/hw/get/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "geo_location",
    "value"     : "13.9, 100.4"
}
```

## Set geo-location or location placement
```
Topic: v1cdti/hw/set/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "set",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "geo_location",
    "value"     : "13.9, 100.4"
}
```

## Monitor machine sensor
```
Topic: v1cdti/hw/monitor/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "monitor",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "wash_count",
    "value"     : "114"
}
```

## Set machie status to "maint" to indicate this machine need to be maintenance.
```
Topic: v1cdti/hw/set/6310301015/model-01/WSH-SN001
Payload: {
    "action"    : "set",
    "project"   : "6310301015",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "status",
    "value"     : "maint"
}
```