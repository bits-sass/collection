# Bits.sass collection

Collection component used for listing items. Useful for listing products'
thumbnails or [Bits.sass group](https://github.com/bits-sass/group) components.

If you need gutter between items, see [Bits.sass space]
(https://github.com/bits-sass/utils-space) or extend the component with
a modifier.

Read more about [Bits.sass toolkit](https://github.com/bits-sass/bits.sass).

## Installation

* __Bower:__ `bower install --save bits-sass-collection`
* __Download:__ [zip](https://github.com/bits-sass/collection/zipball/master),
  [tar.gz](https://github.com/bits-sass/collection/tarball/master)
* __Git:__ `git clone https://github.com/bits-sass/collection.git`

## Demo

See [demo](https://rawgithub.com/bits-sass/collection/master/demo/index.html).

## Available SASS variables

* `bits-components-ns` - components namespace, defaults to 'bits-'

## Available classes

* `Collection` - core collection component
* `Collection--center` - horizontally center all items
* `Collection--middle` - vertically align all items to middle
* `Collection--bottom` - vertically align all items to bottom
* `Collection-item` - descendant class representing an item

## Usage

Simple collection of thumbnails.

```html
<div class="Collection">
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
</div>
```
Collection of thumbnails with a gutter inbetween. You need to add a modifier
for gutter or use `u-gutter[T][s]` utility from [Bits.sass space]
(https://github.com/bits-sass/utils-space) where you add *Collection-item*
to `$bits-space-gutter-supported-children` variable.

```html
<div class="Collection u-gutterAm">
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  <div class="Collection-item">
    <img class="Thumbnail" src="http://lorempixel.com/100/100" alt="">
  </div>
  …
</div>
```

Collection of [Bits.sass group](https://github.com/bits-sass/group).

```html
<div class="Collection u-gutterHm">
  <div class="Collection-item">
    <div class="Group">
      <div class="Group-item">
        <button class="Button">My account</button>
      </div>
      <div class="Group-item">
        <button class="Button">Settings</button>
      </div>
      <div class="Group-item">
        <button class="Button">Logout</button>
      </div>
    </div>
  </div>

  <div class="Collection-item">
    <div class="Group">
      <div class="Group-item">
        <input class="FormControl" type="text">
      </div>
      <div class="Group-item">
        <button class="Button">Send</button>
      </div>
    </div>
  </div>

  <div class="Collection-item">
    <div class="Group">
      <div class="Group-item">
        <button class="Button">I'm alone</button>
      </div>
    </div>
  </div>
</div>
```

## Requirements

* Sass 3.2+

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 8+