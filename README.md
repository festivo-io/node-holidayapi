# node-holidayapi
Official Node.js library for [HolidayAPI.pl](https://holidayapi.com)

## Installation

```shell
npm install --save holidayapi-node
```

## Usage

```javascript
let HolidayAPI = require('holidayapi-node');
let hApi = new HolidayAPI('YOUR_API_KEY').v1;

let parameters = {
  // Required
  country: 'PL',
  year:    2019,
  // Optional
  // month:    7,
  // day:      4,
  // previous: true,
  // upcoming: true,
  // public:   true,
  // pretty:   true,
};

hApi.holidays(parameters, function (err, data) {
  // Insert awesome code here...
});
```

