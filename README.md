
Compass Sprite
=================

> SASS mixin to generate sprites (using [Compass](http://compass-style.org/) and placeholders)

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

    // Into .class-name:before
    @include sprite(imageName before); @extend %iconBefore;

    // Into .class-name:after
    @include sprite(imageName after); @extend %iconAfter;
}
````

## Installation

1. Add ````_image.scss```` to yours mixins
2. Check ````sass_dir```` in your ````config.rb```` and add ````relative_assets = true````
3. Copy settings, change directories of images and call the mixin
4. Import ````_sprite.scss```` in your stylesheet