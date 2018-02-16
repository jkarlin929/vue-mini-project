# Vue.js

[Link to CodeSandbox](https://codesandbox.io/s/643v2kmrzw)

-Vue (pronounced like view) is a progressive framework for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects. On the other hand, Vue is also perfectly capable of powering sophisticated Single-Page Applications when used in combination with modern tooling and supporting libraries.   
-Chrome Ext. VueDevTools comes in handy.

# History
Vue was created by Evan You after working for Google using AngularJS in a number of projects. He later summed up his thought process, "I figured, what if I could just extract the part that I really liked about Angular and build something really lightweight without all the extra concepts involved?"[6] Vue was originally released in February 2014.

# Installing
```
npm install -g @vue/cli  
vue create my-project
```

Vue CLI is a full system for rapid Vue.js development, providing:

Interactive project scaffolding via @vue/cli.
Zero config rapid prototyping via @vue/cli + @vue/cli-service-global.
A runtime dependency (@vue/cli-service) that is:
Upgradeable;
Built on top of webpack, with sensible defaults;
Configurable via in-project config file;
Extensible via plugins
A rich collection of official plugins integrating the best tools in the frontend ecosystem.
Vue CLI aims to be the standard tooling baseline for the Vue ecosystem. It ensures the various build tools work smoothly together with sensible defaults so you can focus on writing your app instead of spending days wrangling with configurations. At the same time, it still offers the flexibility to tweak the config of each tool without the need for ejecting.

# Usage
Vue uses an HTML-based template syntax that allows you to declaratively bind the rendered DOM to the underlying Vue instance’s data. All Vue templates are valid HTML that can be parsed by spec-compliant browsers and HTML parsers. Under the hood, Vue compiles the templates into virtual DOM render functions. Combined with the reactivity system, Vue is able to intelligently figure out the minimal number of components to re-render and apply the minimal amount of DOM manipulation when the app state changes.  

In Vue, you can use the template syntax or choose to directly write render functions using JSX. In order to do so just replace the template option with a render function.[7] Render functions open up possibilities for powerful component-based patterns — for example, the new transition system is now completely component-based, using render functions internally.[8]
Usage: vue <command> [options]

Commands:
```
  create [options] <app-name>      create a new project powered by vue-cli-service
  invoke <plugin> [pluginOptions]  invoke the generator of a plugin in an already created project
  inspect [options] [paths...]     inspect the webpack config in a project with vue-cli-service
  serve [options] [entry]          serve a .js or .vue file in development mode with zero config
  build [options] [entry]          build a .js or .vue file in production mode with zero config
  init <template> <app-name>       generate a project from a remote template (legacy API, requires @vue/cli-init)
```
# Creating a new Project
Usage: create [options] <app-name>

create a new project powered by vue-cli-service


Options:
```
  -p, --preset <presetName>       Skip prompts and use saved preset
  -d, --default                   Skip prompts and use default preset
  -i, --inlinePreset <json>       Skip prompts and use inline JSON string as preset
  -m, --packageManager <command>  Use specified npm client when installing dependencies
  -r, --registry <url>            Use specified npm registry when installing dependencies (only for npm)
  -f, --force                     Overwrite target directory if it exists
  -h, --help                      output usage information

```

```
vue create my-project
```
-after creating a new project, you can use default or manual presets.



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

# Directives
-Directives are prefixed with v- to indicate that they are special attributes provided by Vue, and as you may have guessed, they apply special reactive behavior to the rendered DOM. In the code snippet, v-for declares a for loop for each of the products in our array. The 'product' acts like a parameter in which we call the name of the product from our products array. Everything between the opening and closing li tags are now inside of our 'for' loop.
Writing an if statement is simple, too. Simply, write v-if="Something Something Something". Using a span tag is also something Vue utilizes often, as well.

# Documentation
-Lot's of stackoverflow questions and answers.  
-The Vue.js docs are excellent and can be found here:

[Vue.js Docs](https://vuejs.org/v2/guide/index.html#Declarative-Rendering)
