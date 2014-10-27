
Compass Sprite
=================

> SCSS mixin to generate sprites (using [Compass](http://compass-style.org/) and placeholders)

## Usage

````
.class {
    // Into the element
    @include sprite(imageName); @extend %iconElem;
}
````

To insert image in pseudo-element :

````
.class {

    // Into .class:before
    @include sprite(imageName before); @extend %iconBefore;

    // Into .class:after
    @include sprite(imageName after); @extend %iconAfter;
}
````

## Installation

1. Add ````_image.scss```` to yours mixins
2. Check ````images_dir```` in your ````config.rb```` and add ````relative_assets = true````
3. Copy settings, change directories of images and call the mixin

That's all ! But try to use all icons in one global file.
