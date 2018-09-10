### General info:
 - Each object has id and value: `a = 5; id(a)`
 - Mutable (dict, list) and immutable (string, integer, tuple) objects
 - integer division = / (// in Python3): `3/4 == 0; 3/4. == 0.75`
 - __add__, __div__ -  methods which define +, / logic for the object
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
List | Mutable, ordered, array-replacement | `[]` or `list((items...))` | `l[0]="v"; l.append("v"); l.extend((list2...)); l.insert(0,"v")` | `l.[0]="v"; ` | `l.remove("v"); l.pop(index?); del l[0]; l.clear()` | `int count("v"); int index("v"); inplace reverse(); inplace sort()`
Tuple | Immutable, ordered | `()` or `tuple((items...))` | - | - | - | `int count("v"); int index("v")`
Set | Mutable, unordered, unindexed | `{}` or `set((items...))` | `s.add("v")` | `s.update(["v1", "v2"])` | `remove("v") raise error; discard("v"); s.pop(index?)` | `s1.difference(s2) - return diff set; s1.difference_update(s2) - inplace diff; s1.intersection(s2) - return intersection set; s1.intersection_update(s2) - inplace intersection; s1.isdisjoint(s2) - has intersection?; s1.issubset(s2); s1.issuperset(s2); s1.symmetric_difference(s2) - return items which are different in sets; s1.symmetric_difference_update(s2) - inplace; s1.union(sets...)`
Dictionary | Mutable, unordered, indexed | `{k:"v",...}` or `dict((k="v",...))` | | | | 
