# SSRS---expand-column-when-hiding-another-one-

**REQUST**: Hide the column in the tablix depending on the parameter.

**PROBLEM**: Title, header footer and other elements are not alligned when column is hidden.

**SOLUTION**:

1. Terminology:
    a) Column that is beeing hidden depending on the variable: X
    b) Column that we want to expand when column X is hidden: A
2. Duplicate column A and set the width of a new column (column B) to A.width + x.width
3. When hiding column X, hide the column A and show the column B
4. When showing column X, hide the column B and show the column A


**RESULT**:
Report will look like this:

![image](https://user-images.githubusercontent.com/17928370/120065960-57fefc80-c074-11eb-8e9e-24ec49f2a1de.png)


