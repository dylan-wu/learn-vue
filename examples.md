<details><summary>Boiler Plate</summary>
<p>

```html
<head>
  <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
  <div id="app">
    ...
  </div>
</body>
```

```javascript
var app = new Vue({
  el: '#app',
  data:{
  }
})
```

</p>
</details>

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

3. Use v-if to print text and when inputting app.seen = 0 into the console, the text dissapears

<details><summary>Solution</summary>
<p>

```html
<head>
  <script src=" https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
  <div id="app">
    <span v-if="seen">Now you see me</span>
  </div>
</body
```

```javascript
var app = new Vue ({
  el: '#app',
  data: {
    seen: true
  }
})
```

</p>
</details>

4. Use v-for to print a to-do list

<details><summary>Solution</summary>
<p>

```html
<head>
  <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
  <div id="app">
    <ol>
      <li v-for="todo in todos">
        {{ todo.text }}
      </li>
    </ol>
  </div>
</body>
```

```javascript
var app = new Vue({
  el: '#app',
  data: {
    todos: [
      { text: 'Learn JavaScript' },
      { text: 'Learn Vue' },
      { text: 'Build something awesome' }
    ]
  }
})

```

</p>
</details>

5. Use v-on:click to reverse a message

<details><summary>Solution</summary>
<p>

```html
<head>
  <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
  <div id="app">
    <p>{{ message }}</p>
    <button v-on:click="reverseMessage">Reverse Message</button>
  </div>
</body>
```

```javascript
var app5 = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue.js!'
  },
  methods: {
    reverseMessage: function () {
      this.message = this.message.split('').reverse().join('')
    }
  }
})
```

</p>
</details>

# FAQ

1. What is a div?
2. Why can't I print "Hello Vue!" in HTML
3. What is Vue?
