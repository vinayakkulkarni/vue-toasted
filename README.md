<p align="center">
    <a href="https://github.com/shakee93/vue-toasted" target="_blank">
    <img width="250"src="https://freshpixl.com/vue-toasted.png?new">
    </a>
</p> 

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/vuejs/awesome-vue)

## Introduction

vue-toasted is a cool material toast plugin with variety of options and styles. it is touch compatible and responsive.
issues and pr's are always welcome 

Checkout the <a target="_blank" href="https://shakee93.github.io/vue-toasted/"> Interactive Demo </a> here.

<p align="center">
    <img src="https://shakee93.github.io/vue-toasted/assets/images/vue-toasted-demo-x2.gif">
</p>

## Usage

It is simple. couple of lines all what you need.

```bash
# install it via npm
npm install vue-toasted --save
```
```javascript
// register the plugin on vue
import Toasted from 'vue-toasted';

Vue.use(Toasted)

// you can also pass options, check options reference below
Vue.use(Toasted, Options)

```

```javascript
// you can call like this in your component
this.$toasted.show('hello billo')

// and also
Vue.toasted.show('hola billo');
```

All Good Now you have this cool toast in your project.. let's take a look at the api

## API

vue-toasted has methods which makes it much easier to use

### methods
all the below methods return the `Toasted Object` of the toast.
```javascript
Vue.toasted.success( {string | html } message, {object} options)

// available methods
Vue.toasted.show(message, options)
Vue.toasted.success(message, options)
Vue.toasted.info(message, options)
Vue.toasted.error(message, options)
```


#### Toast Object
check the examples to see how to manipulate the object.
```javascript

// html element of the toast
el : HtmlElement

// change text or html of the toast
text : Function(text)

// fadeAway the toast. default delay will be 800ms
goAway : Function(delay = 800)

```

### options

below are the available options

| Option    | Description                                    | Values                  | Default  |
|-----------|------------------------------------------------|-------------------------|----------|
| position  | position of the toast container    | 'top-right', 'top-center', 'top-left', 'bottom-right', 'bottom-center', 'bottom-left' | 'top-right' | 
| duration  | display time of the toast                      |    in millisecond        | null     |
| className | custom css class name of the toast                 |                         |   null       |
| theme | theme of the toast you prefer                       |    'primary', 'outline', 'bubble'                     |   'primary'       |
| onComplete | class name of the optional icon font          |    a callback function               |   null       |


### Credits

+ Whoever contributes to this project :wink:
+ Inspired and developed from [materialize-css](https://github.com/Dogfalo/materialize) toast.


Enjoy Toasting !!
