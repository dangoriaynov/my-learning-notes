### General info:
 - Each object has id and value: `a = 5; id(a)`
 - Mutable (dict, list) and immutable (string, integer, tuple) objects
 - integer division = / (// in Python3): `3/4 == 0; 3/4. == 0.75`
 - `__add__`, `__div__` -  methods which define +, / logic for the object
 - strings with 's', "s", '''s''', """s"""
 - format strings = `"%s".format('t'), "{0}".format('t')`
 - show attrs and methods `dir([]) or dir("")`
 - shows help message for the method `help("a".start_with)`

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
Dictionary | Mutable, unordered, indexed | `{k:"v",...}` or `dict((k="v",...)) or dict.fromkeys((keys...), default_val?)` | `d["k"]="v"; setdefault("k", "def") - create entry if needed, return the key value` | | `del d["k"]; pop("k"); popitem() - removes last item; ` | `values(); items(); keys()`
