# Simple Calculator

The following problem is designed to test and build familiarity with binary trees.

----

### Problem Part 1:

```
Given a binary tree, which contains either a number or an operator compute the result. 
```

Sample input (tree is  viewed by rotating 90 degrees right):
<pre>
  -- 9
 |
+
 |
  -- 3

(9 + 3) = 12
        -- 11
       |
  -- * 
 |     |
+       -- 4
 |
  -- 3

(9 + (11 * 4)) = 53

                  -- 11
                 |
           -- (-)
          |      |
    -- (*)        -- 2
   |      |
(+)        -- 4
   |
    -- 3

(9 + ((11 - 2) * 4)) = 45

</pre>

Notes:

As you can see children are evaluated in the tree before the parents. Therefore a tree with:

<pre>

        -- 9
       |
  -- * 
 |     |
+       -- 1
 |
  -- 2

</pre>

Equates to: 2 + 1 * 9, while

<pre>

        -- 2
       |
  -- + 
 |     |
*       -- 1
 |
  -- 9

</pre>

Equates to (2 + 1) * 9

### Problem Part 2:

```
Given a string which represents a simple equation, build the binary tree representation.
```

### Problem Part 3:

```
Given a binary tree, which contains either a number or an operator compute the result, and a string which represents a simple equation. Modify the tree to correct the order of operations.
```
