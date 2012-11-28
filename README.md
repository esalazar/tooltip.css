#tooltip.css

The tooltip.css project is a pure css implementation of a tooltip element. This css plugin was created in order to allow people to see the power of css3 and become the new standard for tooltips on the web. Also with this css plugin we can hope to remove many bloated javascript implementations of tooltips.

##Implementation

Out implementation is as followed, there is a tooltip element which will be displayed after a hover action is triggered from the container element.

###Usage

You need to include the `tooltip.css` stylesheet and modify your html to have a working tooltip. There are currently two ways to create the tooltip.

#####Tooltip-Parent:

The container and tooltip elements have a parent/child relationship.

```html
<div class="tooltip-parent">
	Container
	<div class="tooltip">
		Tooltip
	<div>
</div>
```

#####Tooltip-Adjacent:

The container and tooltip elements are seperate and adjacent to each other (in case you can't embed the tooltip within the container e.g. an image).

```html
<div class="tooltip-adjacent">
	Container
</div>
<div class="tooltip">
	Tooltip
<div>
```

###Animations

The default animation is set to fade. Currently, the other built-in animation that can be used is a sliding right animation by adding the "tooltip-slide-right" class to the tooltip element.

###Customization

You can create your own animations and override the default time settings by adding your own css.

```css
.tooltip {
	-webkit-animation-duration: 1s;
	-moz-animation-duration: 1s;
	-o-animation-duration: 1s;
	-ms-animation-duration: 1s;
	animation-duration: 1s;
	-webkit-animation-name: custom;
	-moz-animation-name: custom;
	-o-animation-name: custom;
	-ms-animation-name: custom;
	animation-name: custom;
}
```

##Examples

There are several examples (more to come soon) involving tooltip.css in the `/examples` directory.

##Browser Support

The tooltip functionality works on all major browsers. The animations will only work on browsers that support css3 animations. The tooltip will at the least hide/show without any animation if they aren't supported.

##Future Improvements

This is a new side project and there is much work to do! I hope many people will fork and help make this css plugin better!

* New animations for the tooltip.
* Placement of the tooltip relative to the container.
* Improve modularity of the source code.
* Add more trigger states other than hover (like active) for variety.
