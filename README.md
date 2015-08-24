# UIDevice Wrapper for React Native

A wrapper for the native [https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIDevice_Class/index.html#//apple_ref/occ/cl/UIDevice](UIDevice) class allowing you to access device properties and screen dimensions.

## Installation

```
npm install react-native-device --save
```

## Methods

```javascript
Device.isIpad()
```

The device model is of type iPad

```javascript
Device.isIphone()
```

The device model is of type iPhone

## Properties

```javascript
Device.model
```

The device model, such as `iPhone 5` or `iPad Air` - [https://github.com/InderKumarRathore/DeviceUtil/blob/master/DeviceUtil.m](All model options)

```javascript
Device.deviceName
```

The device name, such as `John Smith's iPhone`

```javascript
Device.systemName
```

The device OS name, such as `iPhone OS`

```javascript
Device.systemVersion
```

The device OS version, such as `8.4`

## Example

```
'use strict';

var Device = require('react-native-device');

var ExampleApp = React.createClass({
  render: function() {
    if (Device.isIpad()) {
      // return iPad layout
    } else {
      // return iPhone layout
    }
  }
});
```
