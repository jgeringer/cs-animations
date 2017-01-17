# cs-animations

##transitions
using multiple transitions...
``transition: <property> <duration>, <property> <duration>;

all transition properties...
``transition: <property> <duration> <timing-function> <delay>;

defaults: duration is the only property required...
``transition: <property:all> <duration> <timing-function:ease> <delay:0>;

Fastest transition seen by the human eye is .256 seconds. So don't go faster.

###transition position

###transition visibility
use visibility and opacity to transition something from hidden. this way it will transition both in and out.
if only going off of opacity, it will only fade in.


##transforms

###transforming rotate
can be: rotated, translated(moved across an axis), scaled, skewed

##keyframes

There are two parts to keyframe animations:
1. Create the animation
2. Assign the animation

Keyframe Recipe...
@keyframes <name-animation> {
    <step 1> { <property>: <value>; }
    <step 2> { <property>: <value>; }
}

Target the animation...
#element{
    animation: <name-animation> <duration> <delay> <iteration> <timing-function-ease>;
}

 forwards: makes it so that it animates to and stops at the final step in the animation.

##cubic bezier
cubic-bezier(0.17, 0.89, 0.32, 1.25)
(Xpos-start-start, Ypos-start-end, Xpos-end-start, Ypos-end-end)