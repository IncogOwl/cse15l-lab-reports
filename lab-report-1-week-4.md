# Failure Inducing Input, Bugs and Symptoms

## How to identify bugs and symptoms using specifc inputs

** Today we will be using three examples wherein a failure inducing output was given. We will be identifying the bugs and symptoms that were present in the code and the relationship between them.**
** We will be using the ```MarkdownParse.java``` present in the repository as our base file for displaying these examples.**

## **Code Example No. 1**

In our first example, we assumed that the input would be correct and would be links only. 
This failure inducing input has a picture link as well. Our current code's output would have included it in the list of links as well since it only checks if the parenthesis and brackets are present and adds the element in between the parenthesis.
The symptom here is the picture name being included as a link in the final output, the bug is the add statement that takes in any element that has brackets and is in between the parenthesis. This is fixed by adding an extra if statement that checks if there isn'r an exclamation point and if the next open bracket is not at zeroeth index.
If this is true then it adds the link to the list.

Here is the link to the test file that caused the bug: [Fail-input File No.1](new-file.md)

Here is the change in the code to correct the bug along with the symptom.

![Correction made as displayed in Commint history](Error1.png)




