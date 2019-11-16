# vue-easy-range-date-picker

> A simple range datepicker based on Vue2

# Installation

```bash
npm install --save vue-easy-range-date-picker
```
# Demo
[Try!](https://codesandbox.io/s/vue-template-kgm6v)

# Usage

## ES6 Modules

```js
import RangeDatePicker from 'vue-easy-range-date-picker';
```

```html
<range-date-picker v-model="dates"/>
```

# Props API
| Props                | Type         | Required | Default     |
| ---------------------| -------------| -------- | ------------|
| v-model(1)           | String       | yes      | -           |
| language(2)          | String       | no       | 'zh'        |
| colorToday(3)        | String       | no       | '#41b883'   |
| colorSelected(3)     | String       | no       | '#34495e'   |
| colorActive(3)       | String       | no       | '#41b883'   |

(1) v-model: Bind to an Object data to store the result of dates you selected: 
```js 

dates: 
{ 
    start: 1573052400000, // example
    end: 1574434800000    // example
}
```
Since the type of the output is timestamp, you are supposed to use the `parseTime` function provided in `/src/util.js` to make the result a specified format such as '2019-11-3'

(2) language: Now supporting: Chinese('zh'), Japanese('jp'), English('en')

(3) See how to use: [Try!](https://codesandbox.io/s/vue-template-kgm6v)

# Events

`closePicker` event is emitted when both the start date and end date were selected.

# Build Setup
``` bash
# install dependencies
npm install
# serve with hot reload at localhost:8080
npm run dev
# build for production with minification
npm run build
```

# License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)

