
#drawfillpolygon

##Syntax
**drawfillpolygon** (*x*, *y*  : **array** 1 .. * **of** **int**, *n* : **int**, *Color* : **int**)

##Description
The **drawfillpolygon** procedure is used to draw a filled polygon with *n* points. The polygon is described by the points (*x*(1), *y*(1)) to (*x*(2), *y*(2)) to (*x*(3), *y*(3)) and so on to (*x*(*n*), *y* (*n*)). The polygon will be drawn and filled with *Color*. 
To get an polygon outlined in a different color, use **drawfillpolygon** with the *Color* parameter set to the fill color and then call **drawpolygon**  with the *Color* parameter set to the border color.

##Example
This program will create a filled octagon and display it in color 1 and then outline it in color 3.
        setscreen ("graphics")
        var x : array 1..8 of int := init (100, 100, 135, 185, 
                                   220, 220, 185, 135)
        var y : array 1..8 of int := init (100, 150, 185, 185,
                                   150, 100, 65, 65)
        drawfillpolygon (x, y, 8, 1)
        drawpolygon (x, y, 8, 3)
##Details
The PC allows a maximum of 256 points. As well, **drawfillpolygon**  can fail (due to lack of memory). If failure occurs, it will try to draw an outline of the polygon. If that also fails, it will not draw anything. 
The meaning of the *Color* number depends on the current palette. See the **palette** statement.
The screen should be in a "*graphics*" mode. See the **setscreen** procedure for details. If the screen is not in a "*graphics*" mode, it will automatically be set to "*graphics*" mode.

##See also
**[setscreen.html](setscreen)**, **[maxx.html](maxx)**, **[maxy.html](maxy)** and the various **draw** procedures.