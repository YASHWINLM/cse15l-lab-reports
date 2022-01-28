# Week 4 Lab Report

* NOTE: github wouldn't let me revert to the previous versions so the input couldn't be shown for the last two ones

**First Change**

* infinite loop error 

* github history below

![Image](Screenshot%20(39).png)

* link to bad input [here](https://github.com/YASHWINLM/markdown-parse/blob/main/test-file.md)


* the infinite loop prints these two numbers repeadtedly

![Image](Screenshot%20(40).png)

* The bug was the fact that the code would run an infinite loop due to the fact that it was not checking properly. THis was the symptom of the code, the fact that it was not hadeling -1 properly so it would stall out.

**Second Change**

* added checker for the unclosed open parentheses

![Image](Screenshot%20(41).png)

* link to bad input [here](https://github.com/jared-hughes/markdown-parse/blob/main/test-unclosed-bracket.md)

* The bug was that the links were not showns properly when there was a '(' that was mismatched without a ')' to close it. THis was caused by the symptom of the list not continuing and the link being treated as valid with an open and no closed parentheses if there was a open parentheses without a closed on, that was not being handeled correctly

**Third Change**

* parentheses inside a link

* link to bad input [here](https://github.com/jared-hughes/markdown-parse/blob/main/test-parens-inside-link.md)

![Image](Screenshot%20(42).png)

* The bug was the link being treated as valid when there were parentheses open and closed inside the example link. This was caused by the symptom of the closed parentheses being after the open one beig treated as valid as the if statmentw as ignoring that previously

