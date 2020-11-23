# meny / 3D菜单

**Created by Hakim El Hattab (http://hakim.se, @hakimel)**

<br/>

### Features

- √ ES module
- √ 0 dependency
- √ BEM css

<br/>

### Quick Start
![NPM](https://nodei.co/npm/meny.png)
``` bash
$ yarn add meny
```

<br/>

js

```js
import Meny from 'meny'

Meny.create({
  // The element that will be animated in from off screen
  menuElement: document.querySelector('.meny__menu'),
  // The contents that gets pushed aside while Meny is active
  contentsElement: document.querySelector('.content'),
  // [optional] The alignment of the menu (top/right/bottom/left)
  position: Meny.getQuery().p || 'left',
  // [optional] The height of the menu (when using top/bottom position)
  height: 200,
  // [optional] The width of the menu (when using left/right position)
  width: 384,
  // [optional] Distance from mouse (in pixels) when menu should open
  threshold: 40,
  // [optional] Use mouse movement to automatically open/close
  mouse: true,
  // [optional] Use touch swipe events to open/close
  touch: true,
  angle: 15.5
})
```

> For more details please visit: [Meny](https://github.com/hakimel/Meny)

<br/>

html

```html
<div class="meny__menu">
  menu
</div>
<div class="meny__trigger"/><!--optional-->
<div class="content">
  content
</div>
```

<br/>

css

```css
.meny__menu {
  background-image: linear-gradient(120deg, #e0c3fc 0%, #8ec5fc 100%);;
}

.content {
  background-image: linear-gradient(120deg, #fdfbfb 0%, #ebedee 100%);
  height: 100vh;
}
```
