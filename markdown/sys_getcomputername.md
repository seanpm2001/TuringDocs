
#Sys.GetComputerName

##Syntax
**Sys.GetComputerName** : **string**

##Description
The **Sys.GetComputerName **function is used to determine the name of the computer. On the PC, this is the NetBIOS name. It returns No Name if a name could not be determined.

##Example
This program outputs a greeting to the user .
        var computerName, userName : string
        computerName := Sys.GetComputerName
        userName := Sys.GetUserName
        put "Hello ", userName, " on ", computerName
##Status
Exported qualified.
This means that you can only call the function by calling **Sys. GetComputerName**, not by calling **GetComputerName**.

##See also
**[sys_getusername.html](Sys.GetUserName)** to obtain the user name of the user currently logged in.