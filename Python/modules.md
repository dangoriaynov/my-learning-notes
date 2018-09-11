### copy
 - `copy()` - return a shallow copy of the object (1-level deep copy)
   to change the logic redefine `obj.__copy__()` method
 - `deepcopy()` - make a deep copy of the object (copy all referenced objects)
   to change the logic redefine `obj.__deepcopy__(dict)` method
   memo dict shows list of already copied referenced objects 
