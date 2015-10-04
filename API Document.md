
#API
    $(selector).rotate();
    $(selector).scale();
    $(selector).translate();
    $(selector).transform2D();

Get specific 2D transform data of the jQuery element. 

- rotate(): Rotation value in degree
- scale(): Array of scale ratio: 
  + *scale X*
  + *scale Y*
- translate(): Array of translate (unit: pixel):
  + *translate X*
  + *translate Y*
- transform2D(): Object includes all transform data
  + *rotate*
  + *scaleX*
  + *scaleY*
  + *translateX*
  + *translateY*

<div><br></div>

    [jQuery Element].rotate(degree);
Rotate the element clockwise.  
*Argument format: see note below*

<div><br></div>

    $(selector).scaleX(ratio);
    $(selector).scaleY(ratio);
    $(selector).scale(ratio);
    $(selector).scale(ratioArr);
Scale the element.

- **scaleX(ratio)**: Scale in X-axis.
- **scaleY(ratio)**: Scale in Y-axis.
- **scale(ratio)**: Scale in both X-axis and Y-axis.
- **scale(ratioArr)**: Scale in X-axis and Y-axis separately. *ratioArr: [scaleX, scaleY]*

*Argument format: see note below*

<div><br></div>

    $(selector).translateX(offset);
    $(selector).translateY(offset);
    $(selector).translate(offsetArr);
Offset the element.

- **translateX(ratio)**: Offset in X-axis.
- **translateY(ratio)**: Offset in Y-axis.
- **translate(offsetArr)**: Offset in X-axis and Y-axis separately. *offsetArr: [offsetX, offsetY]*

*Argument format: see note below*

<div><br></div>

    $(selector).transform2D(opts);
Transform the element by given options.
 
- **opts**
  + rotate
  + scaleX
  + scaleY
  + translateX
  + translateY


*Argument format: see note below*

<div><br></div>

> **Argument Format:**  
You can transform the element by 2 kinds of value:  
1. Number: Set the transformation of the given value.  
2. String start with "+=" or "-=" and following by a number: Adjust the transformation value from current situation by given value.

<div><br></div>