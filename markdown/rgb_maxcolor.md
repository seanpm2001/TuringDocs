
#RGB.maxcolor

##Syntax
**maxcolor** : **int**

##Description
The **maxcolor** function is used to** **determine the maximum color number for the current mode of the screen. The alternate spelling is **maxcolour**.

##Example
This program outputs the maximum color number.
        setscreen ("graphics")
        
        put "The maximum color number is ", maxcolor
##Details
The screen should be in a "*screen*"* *or "*graphics*" mode. If it is not, it will automatically be set to "*screen*" mode. See **View.Set **for details.
For IBM PC compatibles in "*screen*"* *mode, **maxcolor** = 15. For the default IBM PC compatible "*graphics*" mode (CGA), **maxcolor** = 3.

##Status
Exported unqualified.
This means that you can call the function by calling **maxcolor** or by calling **RGB.maxcolor**.

##See also
**[draw_dot.html](Draw.Dot)** for examples of the use of **[maxcolor.html](maxcolor)**. See the **[text_color.html](Text.Color)** [procedure.html](procedure) which is used for setting the currently-active [color.html](color).