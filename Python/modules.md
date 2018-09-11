### copy
Make shallow or deep copy of obj and its references
**Features:**
 - Change the copy logic by re-defining the `obj.__copy__()` method
 - Change the deep copy logic by re-defining the `obj.__deepcopy__(dict)` method,
   memo dict shows list of already copied referenced objects 
**Signature:**
 - `copy()` - return a shallow copy of the object (1-level deep copy)  
 - `deepcopy()` - make a deep copy of the object (copy all referenced objects)   
   

### pickle
  General marshaling / unmarshaling, picking / unpickling in **binary format**
  **Features:**
  - track objects already serialized
  - support self-references
  - support object sharing (multiple referenced to the same object)
  - transparent picking/unpickling of user-defined classes (class should be in the same module as on time object was stored)
  - always backward-compatible across Python releases
  - basic types, top-level functions, lambdas and classes and their derivatives may be pickled
  - when pickling the methods/functions - only their full names are pickled, not the implementation itself
  - when class objects are pickled - no internal data is stored
  - when the instance is pickled - no class data/functions is stored with him, only instance methods are stored
  **Signature:**
  - `DEFAULT_PROTOCOL == 3` for Python3
  - `0 <= DEFAULT_PROTOCOL <= HIGHEST_PROTOCOL`
  - `dump(obj, file, protocol=None, *, fix_imports=True) or Pickler(file, protocol=None, *, fix_imports=True).dump(obj)` - write bytes representation of the object to file (w open for binary), `fix_imports` - make result compatible with Python2
  - `dumps(obj, protocol=None, *, fix_imports=True)` - return the bytes representation of object
  - `load(file, *< fix_imports=True, encording='ASCI', errors='strict') or Unpickler(file, *, fix_imports=True, encoding="ASCII", errors="strict").load()` - unpickle from file to the reconstituted object
  - `loads(bytes_object, *, fix_imports=True, encoding="ASCII", errors="strict")` - unpickle from bytes_object

### pickletools
  Analyse pickled data
  **Features:**
  **Signature:**
  - `optimize()` - generate more compact pickles

### marshal
  Serialization / deserialization for .pyc files
  - serialize the same objects again
  - will crash on self-referenced object
  - no support for object sharing
  - no support for user-defined classes
  - no guarantee to be portable across python versions
  
## json
  Searialization / deserialization in **text**
  - human-readable
  - not python-specific
  - can serialize only subset of python built-in types
