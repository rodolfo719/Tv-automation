# Device Registry Service

## Usage

All response will have the form

```json
{
    "data": "Mixed type holding the content of the response",
    "message": "Description of what happened"
}
```

Subsequent response definitions will only detail the expected value of the `data field`

### List all devices


`GET /devices`

**Response**

- `200 OK` on success
```json
[
  {
      "identifier": "floor-lamp",
      "name": "Floor Lamp",
      "device_type": "switch",
      "controller_gateway": "192.168.0.2"
  },
  {
      "identifier": "samsung-tv",
      "name": "Living Room TV",
      "device_type": "tv",
      "controller_gateway": "192.168.0.9"
  }
]
```
