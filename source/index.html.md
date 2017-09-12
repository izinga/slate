---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - python

toc_footers:
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
# Get All Devices

import requests
response = requests.get("http://localhost:8085/v2/devices")
response.json()
```


This endpoint retrieves all devices.


## Get a Specific Device
> replace device_id with your device id.

```python
# Get a Specific Device

import requests

response = requests.get("http://localhost:8085/v2/device/<device_id>")
response.json()
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

