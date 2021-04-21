# *CSS*
## *css transform*
+ ## *The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.*
+ ## *transform syntax: its include the transform property and the value.*

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

## *2D transforms:*
+ ## *2D rotate: The rotate value provides the ability to rotate an element from 0 to 360 degrees.*

```
.box-1 {
  transform: rotate(20deg);
}
```

+ ## *2D scale: allows you to change the appeared size of an element.*

```
.box-1 {
  transform: scale(.75);
```

+ ## *2D translate: pushing and pulling an element in different directions without interrupting the normal flow of the document.*

```
.box-3 {
  transform: translate(-10px, 25%);
}

```

+ ## *2D skew: distort elements on the horizontal axis, vertical axis, or both.*

```
.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}
```

+ ## *you can combine more than one transform togather:*

```
.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}
```

## *3D Transforms:*
+ ## *3D rotate: like the 2D rotate but with value of rotateX or Y or Z.*

```
.box-1 {
  transform: perspective(200px) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) rotateY(45deg);
}
.box-3 {
  transform: perspective(200px) rotateZ(45deg);
}
```

+ ## *3D scale: by using scaleZ.*

```
.box-1 {
  transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) scaleZ(.25) rotateX(45deg);
}
```

+ ## *3D skew: skew is a two dimentional transform that cannot be transformed to 3D dimentions.*

# *transitions and animations.*
## *transition:  for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.*

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

```
.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  .box:hover {
    background: #ff7b29;
    border-radius: 50%;
  }
```

## *not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another.*



# [back](../README.md)