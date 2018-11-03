# Hello Vue

1. Use Vue to print Hello Vue!

Vue.js cdn: https://cdn.jsdelivr.net/npm/vue/dist/vue.js

<details><summary>Solution</summary>
<p>

```html
<head>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
    <div id="app">
        {{ message }}
    </div>
</body>
```

```javascript
var app = new Vue({ 
    el: '#app',
    data: {
        message: 'Hello Vue!'
    }
});
```

</p>
</details>

2. Use Vue to cause hovering over text to show the time and date the page was loaded on

<details><summary>Solution</summary>
<p>

```html
<head>
  <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
  <div id="app">
    <span v-bind:title="message">
      Hover your mouse over me for a few seconds
      to see my dynamically bound title!
    </span>
  </div>
</body>
```

```javascript
var app = new Vue({
  el: '#app',
  data: {
    message: 'You loaded this page on ' + new Date().toLocaleString()
  }
})
```

</p>
</details>
