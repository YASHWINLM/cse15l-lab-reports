# Lab 5

**Running tests**

* We created a script to search through the tests that looked like this

`for file in test-files/*.md;
do
  echo $file
  java MarkdownParse $file
done`

* then we put the results in the results.txt file just for storage

`bash script.sh > results.txt`

* used the diff command to compare the different implementations of markdown-parse

**1st difference(#14)**

![Image](Screenshot%20(82).png)

* For this difference our implementation did not find a valid link, so the array was empty, as shown below but the other implementation returned a single link with /foo

![Image](Screenshot%20(83).png)

* here is the expected output: 

![Image](Screenshot%20(85).png)

* Our implementation should be correct becasue it actually checked for backslash escape characters whereas the other one did not

* In order to solve this the other implementation should be checking for a backslash escape character, which is why our code did not have a link. By adding in a check for the backslash escape characters to line 35 in a similar format to how we checked for the brackets and parentheses would fix the issue. Where the logic would be to check for a \ within the brackets, else continuing to the next bracket.

![Image](Screenshot%20(84).png)


~~


**2nd difference(#22)**

![Image](Screenshot%20(86).png)

* For this difference our implementation did find a valid link, whereas the other on did not find a valid link

![Image](Screenshot%20(87).png)

* here is the expected output: 

![Image](Screenshot%20(88).png)

* Our implementation should be correct becasue it is checking and finding the link, which shows up in the actual output for the test

* In order to solve this the other implementation I think that changing the logic at line 42 would fix the issue, becuase currently it seems like the star character is causing some issues for the MDP, meaning that the lack of a period and the star seems to invalidate the link in the other implementation, so by adding some checks for a star as well as allowing links without periods in them to be considered valid the other implementation can be fixed.

![Image](Screenshot%20(89).png)






