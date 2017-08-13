## Project Install

# npm

npm install vuetify

## Use

import Vue from 'vue'

import Vuetify from 'vuetify'

Vue.use(Vuetify)

> For including styles, you can either place the below styles in your index.html

    <link href='https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons' rel="stylesheet">

> And for css you can import in entry file 

    import 'vuetify/dist/vuetify.min.css'

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
