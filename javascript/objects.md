# Objects


call by reference in objects

When we pass an object as a parameter to a function the object is not copied to the parameter but is referenced to the parameter. 
So if we try to change the values of properties using the argument we also change the value of the property in the object itself.

This happens because the object memory location is being referenced in the parameter not the object. as both the top-level and block-level variables access the object using the same memory location the objects value get changed even inside the block level scope.