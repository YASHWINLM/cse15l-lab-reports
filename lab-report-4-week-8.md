# Week 8 Lab report 4

**Snippet 1**

[our repo](https://github.com/YASHWINLM/markdown-parse)
[their repo](https://github.com/m1ma0314/markdown-parse)

* Correct output: [`google.com, google.com, ucsd.edu]

Us

![Image](Screenshot%20(62).png)

* Small change?

No need as the test passed

Them

There is a simple change that can be made in order to fix this failure. The fix would be to add a checker for a [ ] in side the ( ) this is becuase right now the link is being treated as if the link called co[de is the same url as code, this is because the [ inside the naming area is not being checked for properly.

![Image](Screenshot%20(69).png)

* Small change?

**Snippet 2**

* Correct output: [a.com, a.com(()), example.com]

Us

![Image](Screenshot%20(63).png)

* Small change?

There is a small change that I could make to fix the incorrect output. This is because the error is with the inclusion of the parentheses, which could be fixed by modifying the way that our check for closed parentheses work, which would be less than 10 lines.

Them

![Image](Screenshot%20(70).png)

* Small change?

There is a small change that could mend this failure of the test for snippet 2. This fix would be to change the way that they handle the ) inside of the link due to the fact that it currently is skipping them.
**Snippet 3**

* Correct output: [https://www.twitter.com, https://ucsd-cse15l-w22.github.io/, https://cse.ucsd.edu/]

Us

![Image](Screenshot%20(65).png)

* Small change?
I don't think there is a small change that I could make in order to fix this error. The index out of bounds exception indicates that one of my for loops is written incorrectly which means that I would likely have to scrap and rewrite it so that change would be over 10 lines of code.

Them

![Image](Screenshot%20(71).png)

* Small change?

I think there is a small change that could be made in order to fix this error. The index out of bounds exception is caused by the adding of their extra variables in the loop, meaning that if the values in the loop are adjusted the index out of bounds error should be fixed.