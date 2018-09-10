### General info:
 - Each object has id and value: `a = 5; id(a)`
 - Mutable (dict, list) and immutable (string, integer, tuple) objects
 - integer division = / (// in Python3): `3/4 == 0; 3/4. == 0.75`
 - `__add__`, `__div__` -  methods which define +, / logic for the object
 - strings with 's', "s", '''s''', """s"""
 - format strings = `"%s".format('t'), "{0}".format('t')`
 - show attrs and methods `dir([]) or dir("")`
 - shows help message for the method `help("a".start_with)`
 - `if-elif-else` clause
 - `try-except-else-finally` clause
 - `import json; json.loads("json content"); json.dumps(json_var)`
 - in statement - `try __contains__ except: __iter__`
 - docstring - string after func/class name, invoke by `__doc__` or `help(method)`
 - `is_instance(var, class)`
 - `3 < x < 5` is replacement for `3 < x and x < 5`
 - range - half-open interval `range(1,3) == [1,2]`, end-start==length
 - enumerate(list) if need to have index+value while iterating
 - slicing `a=range(5); a[-1]==4; a[1:3]==[1,2]; a[1,4,2]==[1,3]` - -1 is like length-1
 - `veg='tomatoe'; veg[:-1] - correct; veg[::2]=='tmte'; veg[::-1]=='oetamot'` - [a,b,c] - c is step
 - `with open("file_name") as f: for line in f: print(line)` - file op
 - `import pdb; pdb.set_trace()` - python debugging, `h` - help

### Operators:
 - arithmetic `% - modulus, ** - exp, // - floor division`
 - assignment `=, -=, +=, *=, /=, %=, **=, //=, &=, |=, ^=, >>=, <<=`
 - comparison `==, !=, >=, <=, >, <`
 - logical `and, or, not`
 - identity `is, is not`
 - membership `in, not in`
 - bitwise `&, | , ^ (XOR, only 1 is true), ~ (not), << (left shift), >> (right shift)`
 
### Data structures
Name | Features | Constructor | Assign | Modify | Delete | Other
--- | --- | --- | --- | --- | --- | ---
List | Mutable, ordered, array-replacement | `[]` or `list((items...))` | `l[0]="v"; append("v"); extend((list2...)); insert(0,"v")` | `l.[0]="v"; ` | `remove("v"); pop(index?); del l[0]; clear()` | `int count("v"); int index("v"); inplace reverse(); inplace sort()`
Tuple | Immutable, ordered | `()` or `tuple((items...))` | - | - | - | `int count("v"); int index("v")`
Set | Mutable, unordered, unindexed | `{}` or `set((items...))` | `add("v")` | `update(["v1", "v2"])` | `remove("v") raise error; discard("v"); pop() - last item` | `difference(s2) - return diff set; difference_update(s2) - inplace diff; intersection(s2) - return intersection set; intersection_update(s2) - inplace intersection; isdisjoint(s2) - has intersection?; issubset(s2); issuperset(s2); symmetric_difference(s2) - return items which are different in sets; symmetric_difference_update(s2) - inplace; union(sets...)`
Dictionary | Mutable, unordered, indexed | `{k:"v",...}` or `dict((k="v",...)) or dict.fromkeys((keys...), default_val?)` | `d["k"]="v"; setdefault("k", "def") - create entry if needed, return the key value` | | `del d["k"]; pop("k"); popitem() - removes last item; ` | `values(); items(); keys(); get("k", default?) - None if no default`

cudos:
- https://www.slideshare.net/MattHarrison4/learn-90
- https://www.w3schools.com/python/default.asp
