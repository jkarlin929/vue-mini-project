# Vue.js

-Vue (pronounced like view) is a progressive framework for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects. On the other hand, Vue is also perfectly capable of powering sophisticated Single-Page Applications when used in combination with modern tooling and supporting libraries.
-Chrome Ext. VueDevTools comes in handy.

[Link to CodeSandbox](https://codesandbox.io/s/643v2kmrzw)

### HTML
```                                         
<div id="app">
  {{ message }}
</div>
```

### JavaScript
```
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue!'
  }
})
```

### Renders:

    Hello Vue!

The data and the DOM are now linked, and everything is now reactive

[A Code Snippet](http://res.cloudinary.com/jkarlin929/image/upload/v1518737261/vue-code_a4moh2.png)

[Another Code Snippet](http://res.cloudinary.com/jkarlin929/image/upload/v1518738230/vue-code-2_i98itv.png)

#Directives
-Directives are prefixed with v- to indicate that they are special attributes provided by Vue, and as you may have guessed, they apply special reactive behavior to the rendered DOM. In the code snippet, v-for declares a for loop for each of the products in our array. The 'product' acts like a parameter in which we call the name of the product from our products array. Everything between the opening and closing li tags are now inside of our 'for' loop.
Writing an if statement is simple, too. Simply, write v-if="Something Something Something". Using a span tag is also something Vue utilizes often, as well.

#Documentation
-Lot's of stackoverflow questions and answers.
-The Vue.js docs are excellent and can be found here:

[Vue.js Docs](https://vuejs.org/v2/guide/index.html#Declarative-Rendering)
