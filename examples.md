# Hello Vue

1. Use Vue to print Hello Vue!

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
ar app = new Vue({ 
    el: '#app',
    data: {
        message: 'Hello Vue!'
    }
});
```

</p>
</details>
