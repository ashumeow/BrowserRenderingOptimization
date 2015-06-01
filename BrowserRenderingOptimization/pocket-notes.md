```
R => Response
A => Animate
I => Idle
L => Load

Response => 100 ms,
Animate => 16ms,
Idle => 50ms,
Load => 1 second
```
```
F => First
L => Last
I => Invert
P => Play
```
Some examples for FLIP mechanism towards RAIL
```js
// Read collapsed positions
this.collectProperties_(this.collapsedPositions_);

// Expand the card and read again
this.elements_.root.classList.add('card--expanded');
this.collectProperties_(this.expandedPositions_);

// Figure out the difference and transform back
this.calculatePositionDiffs_();
this.setElementTransformsToStartAndClipToCollapsed_();

// Wait a frame
requestAnimationFrame(function() {
// Switch on animation and remove the transforms
this.elements_.root.classList.add('card--animatable');
this.setElementTransformsToZeroAndClipToExpanded_();
});
```
