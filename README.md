# ion-number-picker

An ionic number picker (spinner) which is developed in web technologies and Angular but looks similar to native.

## Requirements

- Works with Angular 1.*

## ScreenShots
![alt tag](/screenshots/screenshot1.gif)
![alt tag](/screenshots/screenshot3.png)

## Usage

- Add CSS and JS to project:

```html
<link rel="stylesheet" href="wherever-you-put-it/ionNumberPicker.min.css">

<script type="text/javascript" src="wherever-you-put-it/ionNumberPicker.min.js"></script>
```

Add dependencies on the `ion-number-picker` AngularJS module:

```javascript
angular.module('myApp', ['ion-number-picker']);
```

You can now use the directive, add the attribute to your existing DOM element in HTML:
```html
<input type="text" ng-model="value" ion-number-picker>
```

## Directive Attributes

- `id (optional)` - Give a unique id the the bound element and drawer will be named {{id}}-drawer. Default is randomly generated id
- `ng-model (optional)` - Define the model to bind the selected value to. the value of the model is displayed once drawer is open.
- `ng-change (optional)` - method called after the value has been set
- `sensitivity (optional)` - Define the scroll sensitivity. default is 0.17
- `min` (optional) - define the first top value of the number selector. Default is 1
- `max` (optional) - define the last bottom value of the number selector. Default is 100
- `ngDefault` (optional) - if ng-model is null then number selector open on this number as selected. Default is minimum value
- `step` (optional) - define the step between the first and last values. Can be a float number or negative value. Default is 1
- `control` (optional) - control element to control directive from outside (see notes below for details)
- `hasClear` (optional) - true/false Whether drawer has clear button or not, if does value set to null. Default is false.
- `onSet` (optional) - event fired when set button clicked, model is set value. Has two params oldValue and newValue, If returning false from method set canceled. IMPORTANT: only pass method name without brackets
- `onCancel` (optional) - event fired when cancel button clicked. IMPORTANT: only pass method name without brackets
- `onClear` (optional) - event fired when clear button clicked. IMPORTANT: only pass method name without brackets


## Notes

Valid values:
- Make sure you enter number values for start, end, and step.
- Total number of elements is limited to 4000 for user experience considerations
- Control methods which can be called:
 * `openDrawer` - opens the number select drawer
 * `closeDrawer` - closes the number select drawer
 * `getCurrentSelection` - returns the current value displayed as selected in number select drawer
 * `isDrawerOpen` - is the drawer currently open or not

## Purchase Link
[ion-number-picker](https://gum.co/uEFnY)

## What's included
Upon purchase you'll receive a minimized js file and minimized css for immediate use

## License
Use only by person/business specified in payment for one or more end products
TODO
