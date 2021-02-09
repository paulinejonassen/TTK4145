
The magic numbers is unpredictible. The number variates from -1 000 000 to 1 000 000.  
The reason for that is that the program runs the  functions simultainiously. The functions uses a global variable, which is shared between the functions. Which means that the functions will be reading and writing to the variable at the same time, and changing the variable before the other function is done writing the new value to the variable.
