---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - python

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

While there is no denying that good documentation is a living entity and many a times we have to write documentation for things that are still under development, we sincerely hope our manager did not force the document writer to write the documentation as written by Alice above. With the caveats out of the way, let us get started with helping you use one of the best app testing platforms that has ever walked the surface of the earth - if it could walk.

RobusTest is designed to be a one stop platform for everyone involved in creating a mobile appication - right from business guys who need to see what their application looks like, to developers who need to run some quick checks to testers who need to test the app extensively using manual and automated methods

# Devices

## Get All Devices


```python
import requests

response = requests.get("http://localhost:8085/v2/devices")
response.json()
```


> The above command returns JSON structured like this:

```json
{
    "available": [
        {
            "_id": "596244f4b996c838ffc76a57",
            "serial": "0123456789ABCDEF",
            "key": "",
            "uiid": "",
            "host": "127.0.0.1",
            "name": "Lenovo A536",
            "brand": "Lenovo",
            "model": "",
            "model_id": "Lenovo A536 - 4.4.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "4.4.2",
            "isConnected": true,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "480x854",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [
                "8951071001",
                "234353446"
            ],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": null,
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Browser",
                    "component": "com.android.browser/.BrowserActivity"
                },
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "_id": "127.0.0.1",
                "name": "Bangalore mac mini",
                "ip": "127.0.0.1",
                "location": "127.0.0.1",
                "status": true,
                "version": false,
                "os": "darwin",
                "serial": "",
                "macAddress": "",
                "created": "2017-08-24T03:01:10.705+05:30",
                "updated": "2017-09-10T21:53:36.726+05:30",
                "last": 1505066975
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1505060616,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        }
    ],
    "busy": [],
    "offline": [
        {
            "_id": "59609077b996c838ffc6f692",
            "serial": "21b7a936d2cdae25bc3ecedf548b3c44c4982a38",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "iPhone 5s",
            "brand": "Apple",
            "model": "",
            "model_id": "iPhone 5s - 10.3.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "10.3.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "0x0",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "iOS",
            "port": 0,
            "screenmode": "default",
            "ratio": 1,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1504523423,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "59649127b996c838ffc8a191",
            "serial": "0255e9ff78752644",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "Nexus 5X",
            "brand": "google",
            "model": "",
            "model_id": "Nexus 5X - 7.1.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "7.1.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "1080x1920",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1499791844,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "5964a2f9b996c838ffc8fe77",
            "serial": "2002cc354587ca26bfe21c0cb36e6f6e6861b9da",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "iPhone 5c",
            "brand": "Apple",
            "model": "",
            "model_id": "iPhone 5c - 10.3.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "10.3.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "0x0",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "iOS",
            "port": 0,
            "screenmode": "default",
            "ratio": 1,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1504888638,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "596debc1023f3553c0142785",
            "serial": "074536210b3008e9",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "Nexus 5",
            "brand": "google",
            "model": "",
            "model_id": "Nexus 5 - 6.0.1",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "6.0.1",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "1080x1920",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1502525117,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        }
    ],
    "reserved": []
}
```

This endpoint retrieves all devices.


## Get a Specific Device
> replace device_id with your device id.

```python
import requests

response = requests.get("http://localhost:8085/v2/device/<device_id>")
response.json()
```


> The above command returns JSON structured like this:

```json
{
    "_id": "596244f4b996c838ffc76a57",
    "serial": "0123456789ABCDEF",
    "key": "0123456789ABCDEF_866566029208777_Lenovo/A536/A536:4.4.2/KOT49H/A536_S186_150813_ROW:user/release-keys",
    "uiid": "",
    "host": "127.0.0.1",
    "name": "Lenovo A536",
    "brand": "Lenovo",
    "model": "Lenovo A536",
    "model_id": "Lenovo A536 - 4.4.2",
    "manufacturer": "",
    "clientidbase": "",
    "countryCode": "",
    "ram": "",
    "fingerprint": "Lenovo/A536/A536:4.4.2/KOT49H/A536_S186_150813_ROW:user/release-keys",
    "version": "4.4.2",
    "isConnected": true,
    "testSession": "",
    "simOperator": "",
    "timezone": "",
    "resolution": "480x854",
    "lcdDensity": "",
    "screensize": "",
    "img": "",
    "numbers": [
        "8951071001",
        "234353446"
    ],
    "useType": [
        "M",
        "A",
        "H"
    ],
    "projects": null,
    "user": "",
    "os": "Android",
    "port": 0,
    "screenmode": "default",
    "ratio": 2,
    "menubar": true,
    "status": false,
    "state": 0,
    "automate": true,
    "browsers": [
        {
            "name": "Browser",
            "component": "com.android.browser/.BrowserActivity"
        },
        {
            "name": "Chrome",
            "component": "com.android.chrome/com.google.android.apps.chrome.Main"
        }
    ],
    "apps": null,
    "display": {
        "width": 480,
        "height": 854,
        "xdpi": 240,
        "ydpi": 240,
        "size": 0,
        "density": 1.5,
        "fps": 54.87,
        "secure": true,
        "rotation": 0
    },
    "imei": "866566029208777",
    "imsi": "",
    "iccid": "",
    "phoneNumber": "",
    "network": "UNKNOWN",
    "reserveKey": "",
    "usage": null,
    "node": {
        "_id": "127.0.0.1",
        "name": "Bangalore mac mini",
        "ip": "127.0.0.1",
        "location": "127.0.0.1",
        "status": true,
        "version": false,
        "os": "darwin",
        "serial": "",
        "macAddress": "",
        "created": "2017-08-24T03:01:10.705+05:30",
        "updated": "2017-09-10T21:53:36.726+05:30",
        "last": 1505067096
    },
    "other": "",
    "minicap": {
        "state": 0
    },
    "minitouch": {
        "state": 0
    },
    "service": {
        "state": 0
    },
    "agent": {
        "state": 0
    },
    "nizedha": {
        "state": 0
    },
    "vnc": {
        "state": 0
    },
    "last": 1505060616,
    "created": "0001-01-01T00:00:00Z",
    "updated": "0001-01-01T00:00:00Z"
}
```
This endpoint retrieves a specific kitten.


### HTTP Request

`GET http://localhost:8085/v2/device/<device_id>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the device to retrieve

<aside class="success">
Remember
<ul>
  <li> isConnected will be true for connected device.</li>
  <li> status will be false for available device.</li>
</ul>
</aside>
## Delete a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.delete(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.delete(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -X DELETE
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint retrieves a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete

