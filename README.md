# quasar-monthpicker
A month picker for Quasar, the Vue.js framework

It looks and behaves very much like Quasar's date picker:

![Screenshot of Quasar MonthPicker](https://louisameline.github.io/quasar-monthpicker/doc/quasar-monthpicker.png)

# Install

```
npm install quasar-monthpicker --save
```
Quasar's Button component is required for this month picker to work. In `quasar.conf.js`:

```
framework: {
  components: ['QBtn']
}
```

# Usage
```javascript
import monthpicker from 'quasar-monthpicker'
export default {
	name: 'periodSelector',
	components: { monthpicker }
}
```
```xml
<monthpicker
	color="purple"
	locale="en-US"
	:min="yourDateObject"
	:max="yourDateObject"
	v-model="yourDateObject"
></monthpicker>
```

# Available props


| Prop                  | Type            | Default     | Description                              |
|-----------------------|-----------------|-------------|------------------------------------------|
| color                 | String          | none, defaults to Quasar's color for buttons    | Color of the selected month           |
| locale                | String          | none, defaults to local language                | The locale passed to Javascript's [`toLocaleTimeString()`](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/Date/toLocaleTimeString) function for the names of months                      |
| max                   | Date object     | none        | Maximum month to select                   |
| min                   | Date object     | none        | Minimum month to select                   |

# Contribute

Merge requests are welcome to help improve this component.
