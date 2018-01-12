# ZANN

[![npm version](https://badge.fury.io/js/zann.css.png)](https://badge.fury.io/js/zann.css)

> _A collection of afterimage effects in CSS animation_

The afterimage effect impresses viewers. The user is exposed to a lot of content, it can not separate important content from other, it is confused every day. This collection exists to make the content that you want to convey more attractive.

## INSTALL

You can install via npm

```
npm install zann.css --save
```

## EASY to USE

Insert link to your website files, and set the `zann.css` reference.

```html
<link rel="stylesheet" href="zann.css">
```

In the case of using CDN hosted.

```html
<link rel="stylesheet" href="https://unpkg.com/zann.css">
```

Just add CSS classes to the element on your website files.

```html
<div class="zann zann-closet--on"></div>
```

Every class has animations of

Modifier | Description
-------- | ----------------------------------
`--on`   | Start animation to turn effect on
`--off`  | Start animation to turn effect off

### CLASSES of EFFECT

- zann-closet
- zann-edge
- zann-ripple
- zann-ripple-back
- zann-scan
- zann-scramble
- zann-slide
- zann-slide-back
- zann-wipe

Please check the behavior on the [demo](https://ai428.github.io/zann.css/) site.

### With VUE.JS

Combined with UI framework like Vue.js, it is more effective. For basic usage of Vue.js, please refer to the wonderful [document](https://jp.vuejs.org/) of the head family.

```html
<!--
This is an example of turning on / off closet effect when clicked. Try it.
-->
<div id="app" @click="isActive = !isActive">
  <div class="zann" :class="{ 'zann-closet--on': isActive, 'zann-closet--off': !isActive }"></div>
</div>

<script src="https://unpkg.com/vue"></script>
<script>
new Vue({
  el: '#app',
  data: {
    isActive: false
  }
});
</script>
```

This is an example of turning on / off closet effect when clicked. Try it.

## LICENSE

Free to use under the [MIT](http://www.opensource.org/licenses/mit-license.php) license.
