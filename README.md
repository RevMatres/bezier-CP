# bezier-CP
My take on a bezier curve drawing API in JavaScript.



#### Note:
There is this other thing called "bezier.js", which can be found [here](https://pomax.github.io/bezierjs/).  
It seems that can do lots more than my humble machinery, but I couldn't figure it out.

At least while I'm writing this the documentation isn't that great... Ah, well.



## Well, what is this?
bezier-CP is a javascript package containing a few classes and functions for drawing bezier curves (on an HTML canvas element).

Bezier curves are defined by a set of points, each of which gets one or two **control points**. Those control points are used
to define the curve's smooth shape, while the curve goes through each of the points.

bezier-CP provides functions to calculate the location of such control points, given the points of the curve.

Automation is also supported: given a whole array of points, the control points can be added to those points.


## Usage

bezier-CP includes the following objects for public use:

### createBezierControlPoints()
**createBezierControlPoints()** returns the point Object, that is passed into it, with the addition of cp1 and cp2.

#### Syntax
```javascript
let P1 = {x,y};
P1 = createBezierControlPoints(point, [N1, N2], bezierSmoothFactor=1, cleanUp=true);
```
##### Parameters
**point**  
The point to calculate the control points for.  
Accepts an Objects containing an x and a y property, like `{x: number, y: number}`.

**[N1, N2]**  
The points, that come before and after the point in the bezier curve.  
`N1` is the point *before*, `N2` is the point *after*.  
Both points must contain x and y properties.

The N stands for neighbour.  

**bezierSmoothFactor**  
doodldooo

**cleanUp**  


### createBezierCurve()
#### Syntax

##### Parameters


### endPointHandle()
#### Syntax

##### Parameters


### drawBezierCurve()
#### Syntax

##### Parameters

### bezierPoint
#### Methods
#### Properties
