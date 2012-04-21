
#whatdotcolor

##Syntax
**whatdotcolor** ( *x*, *y* : **int** ) : **int**

##Description
The **whatdotcolor** function is used to determine the color number of the specified pixel. The alternate spelling is **whatdotcolour**.

##Example
This program draws a line which bounces off the edges of the screen and makes a beep when it finds a pixel that has already been colored.
        setscreen ( "graphics" )
        var x, y : int := 0
        var dx, dx : int := 1
        loop
            if whatdotcolor ( x, y ) not= 0 then
                sound ( 400, 50 )
            end if
            drawdot ( x, y, 1 )
            x := x + dx
            y := y + dy
            if x = 0 or x = maxx then
                dx := -dx
            end if
            if y = 0 or y = maxy then
                dy := -dy
            end if
        end loop
##Details
The screen should be in a"*graphics*" mode. If is not set to "*graphics*"*  *mode,  it will automatically be set to "*graphics*" mode. See **setscreen** for details.

##See also
**[drawdot.html](drawdot)**, which is used for setting the [color.html](color) of a pixel. See also **[maxx.html](maxx)** and **[maxy.html](maxy)**, which are used to determine the number of pixels on the screen. See also **[sound.html](sound)**, which causes the computer to make a [sound.html](sound).
See also predefined unit **[viewmodule.html](View)**.