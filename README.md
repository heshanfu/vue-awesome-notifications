[![npm version](https://badge.fury.io/js/vue-awesome-notifications.svg)](https://badge.fury.io/js/vue-awesome-notifications)

# Vue Awesome Notifications

It's a Vue.js version of [Awesome Notifications](https://github.com/f3oall/awesome-notifications) library. **Awesome Notifications** is a lightweight JavaScript library for notifications.

**Demo**: https://f3oall.github.io/awesome-notifications/
![Demo GIF](demo1.gif)

## Install

> **Attention!** This library uses FontAwesome icons, so you either need to make sure that [FontAwesome](http://fontawesome.io/get-started/) is connected to your project, either disable icons, passing the `icons: {enabled: false}` property to options. Also you can preserve icons, setting up a custom template for them via editting `options.icons.template`

```
npm install --save vue-awesome-notifications
```

**In main.js**

```javascript
import Vue from "vue"
import VueAWN from "vue-awesome-notifications"

Vue.use(VueAWN, options)
```

**In any of your files:**

```javascript
this.$awn.success("Your custom message")
```

## Usage of default styles

For easier customization, SCSS version is preffered.

**With SCSS - In your App.vue**

```html
<style lang="scss">
@import '~vue-awesome-notifications/dist/styles/style.scss';
</style>
```

**With CSS - In your App.vue**

```html
<style lang="css">
@import 'vue-awesome-notifications/dist/styles/style.css';
</style>
```

**Or in main.js**

```javascript
require("vue-awesome-notifications/dist/styles/style.css")
```

\*\*

## Customization

You can pass `options` object to initialization function to override defaults. List of available options can be found in [Awesome Notifications README.md](https://github.com/f3oall/awesome-notifications).

**Styles**

If you use SCSS, you can configure styles by redefining variables. List of available variables can be found in [Awesome Notifications repo](https://github.com/f3oall/awesome-notifications/blob/master/src/styles/variables.scss)

Otherwise, if you use 'style.css', you can only override it.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
