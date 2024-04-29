1. Line 12 prints the value 3. At the very end of the `for` loop, the variable `i` has a value of 3 (leading to termination of the loop). Since `var` means it is not block scoped, we are able to access the variable and print out its value.
2. Line 13 prints the value 150. The variable `discountedPrice` is also a `var`, meaning it is accessible outside the loop. At the end of the loop, it has a value of `150`, since that is 0.5 x 300 (the last value in the array).
3. Line 14 prints the value 150. The variable `finalPrice` is declared in the scope of Line 14, and also it is a `var`, so it is accessible. It takes on the same value as `discountedPrice` and gets rounded, so it remains 150.
4. The function returns an array containing the discounted price of each element in the input array. In the example given, it returns [50, 100, 150], since the input array was [100, 200, 300] and the discount rate was 0.5. In the `for` loop, the variable `i` iterates through the length of the input array. For each index `i`, the discountedPrice is calculated and pushed into the `discounted` array. That is the array that is finally returned.
5. Line 12 throws an error. The variable `i` is defined using `let`, meaning it is block scoped in the `for` loop it is declared with. Since the `console.log` statement tries to print `i` after the `for` loop, `i` is no longer defined in that scope, and therefore an error is thrown.
6. Similar to the previous question, Line 13 also throws an error. The variable `discountedPrice` is block scoped within the previous `for` loop, and so it is not defined outside. Then, when the `console.log` statement tries to access it, an error is thrown.
7. Line 14 prints the value 150. While `finalPrice` is declared with `let`, it is within the scope of Line 14, so we are able to access its value.
8. This function still returns an array containing the discounted version of the input array, which is [50, 100, 150] in our example. The reasoning is the exact same as the Question 4. Changing the variables from `var` to `let` does not change their role in the calculations.
9. Just like Question 5, Line 9 here throws an error. The variable `i` is still defined using `let`, meaning it only exists in the scope of the `for` loop. Trying to access it on Line 9 throws an error.
10. Line 12 prints the value 3. At the very beginning, the variable `length` is defined to be the length of the input array, which in our example is 3.
11. The function returns [50, 100, 150], which is the discounted version of the input array. Similar to the previous examples, the loop iterates through the array and computes the discount of each element. Then, that version is pushed to `discounted`, which is the array that is returned.
12. The responses are:

    A. `student.name`

    B. `student.['Grad Year']`

    C. `student.greeting()`

    D. `student['Favorite Teacher'].name`

    E. `student.courseLoad[0]`

13. The results are:

    A. '32'; the integer 2 maps to the string representation, and the two strings concatenate

    B. 1; the string '3' maps to the integer 3 (Javascript knows this because you cannot subtract strings), and the integers are subtracted

    C. 3; null maps to the integer 0, which is added to 3

    D. '3null'; null maps to the string 'null', and the two strings concatenate

    E. 4; true maps to the integer 1, which is added to 3

    F. 0; false maps to the integer 0, and so does null, leading to 0 + 0 = 0

    G. '3undefined'; undefined maps to the string 'undefined', and the two strings concatenate

    H. NaN; since you cannot subtract two strings and Javascript is unable to map both '3' and undefined to a common type, the reuslt is NaN

14. The results are:

    A. true; the string '2' gets mapped to the integer 2, which is greater than 1

    B. false; as strings, the first two characters are compared, and the character 2 is less than the character 1

    C. true; Javascript converst the type of the variables so that they match, and then compares them

    D. false; when using the '===' operator, types are not converted, meaning 2 and '2' are not the same

    E. false; true gets mappd to its integer value of 1, which is not equal to 2

    F. true; the phrase Boolean(2) gets evaluated to true (any value greater than 0 is true), which is the same type and equal to the left hand side of the operator

15. The '==' operator converts types of variables to the same type before comparing them, while '===' only evaluates to true if both variables are the same type.
16. Response is in `part2-question16.js`
17. The result is [2, 4, 6]. In the `modifyArray` function, we iterate through the input array [1, 2, 3]. For each element in the array, we call `doSomething`, which returns twice the passed in value. So, for 1, the returning value is 2. Each returned value is added to the `newArr`, which is finally returned. In essence, we double the entire input array and return it.
18. Answer in `part2-question18.js`
19. The output of the above code is 1 4 3 2, all in separate lines.
