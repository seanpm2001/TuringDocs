
#View.maxy

##Syntax
**maxy** : **int**

##Description
The **maxy** function is used to** **determine the maximum value of y for the current graphics mode.

##Example
This program outputs the maximum y value.
        setscreen ("graphics")
        
        put "The maximum y value is ", maxy
##Details
The screen should be in a "*graphics*" mode. If it is not, it will automatically be set to "*graphics*" mode. See **setscreen **for details.
For the default IBM PC compatible graphics mode (CGA), **maxy **= 199.

##Status
Exported unqualified.
This means that you can call the function by calling **maxy** or by calling **View.maxy**.

##See also
**[draw_dot.html](Draw.Dot)** for an example of the use of **[maxy.html](maxy)** and for a diagram illustrating x and y positions. 