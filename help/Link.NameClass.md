# Link.NameClass

This function is intended as a replacement for the system function `⎕NC` in tools that manage code. The name classes are given with decimal fraction, as with a nested argument to `⎕NC`. 

The only difference is that `¯9` is returned for unscripted namespaces (including `#` and `⎕SE` which normally yield a name class of `¯1`), which are linked to directories. Scripted namespaces, which are linked to files, retain the regular value `9.1`. 

#### Right Argument

- item name(s)

#### Optional Left Argument

- namespace where to evaluate names 

#### Result

- name classes of the items, with same shape as argument