---
title: 'brightness'
notes:
  - 'Needs example, usage, spec reference'
readiness: 'In Progress'
relationships:
  applies_to:
    predicate: 'Property of '
    value: apis/image_capture/PhotoSettings
    href: /apis/image_capture/PhotoSettings
  return:
    predicate: 'Returns an object of type '
    value: 'unsigned long'
    href: /apis/image_capture/PhotoSettings
standardization_status: 'W3C Working Draft'
summary: 'This reflects the desired brightness setting of the camera.'
tags:
  - API_Object_Properties
  - API
  - Image_Capture
  - Mobile
  - Needs_Examples
uri: 'apis/image capture/PhotoSettings/brightness'

---
## Summary

This reflects the desired brightness setting of the camera.

Property of [apis/image\_capture/PhotoSettings](/apis/image_capture/PhotoSettings)[apis/image\_capture/PhotoSettings](/apis/image_capture/PhotoSettings)

## Syntax

``` js
var result = photoSettings.brightness;
photoSettings.brightness = value;
```

## Return Value

Returns an object of type unsigned longunsigned long

