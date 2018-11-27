# test-nuxt

> Vuescroll - Nuxt Demo

# How to config?

**Only modify two places.**

1. In `/plugins` fold, add `vuescroll.js` , and write something like this:

```javascript
import Vue from 'vue'
import vuescroll from 'vuescroll'
import 'vuescroll/dist/vuescroll.css'

Vue.use(vuescroll)
```

2. Modify `plugins` property in your `nuxt.config.js`.

```javascript
// Add vuescroll
module.exports = {
  plugins: ['~/plugins/vuescroll']
}
```

3. That's all!
