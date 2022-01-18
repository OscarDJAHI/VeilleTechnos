# VeilleTechnos
https://medium.com/@eshagarg1996/best-practices-for-typescript-coding-8b1ea98d02f8

# 1. Code Limit the length:
Limit the length of code to 500–600 lines in a file and the methods to 20–30 lines.

# 2. Naming convention of variable/method/class names:
Variable Names: camelCase
Example: firstNumber = 12

Constants: UPPER_CASE with underscore ‘_’ between multiple words
Example: const FIRST_NUMBER = 18

Method Names: camelCase
Example: sumOfTwoNumbers()

Class Names: PascalCase
Example: export class EmployeeDetails {}

File Names: lower-case (Separated by ‘-’ if the name is of two/more words)
Example: employee-details

# 3. Mention data types of variables while declaration and for method parameters.
Variable Type
Example: firstNumber: number
Parameter Type
Example:

Data types for method parameters

# 4. Avoid the use of type ‘any’. Create an interface/class instead.
Example:
Let’s assume that we need to assign the details of a person to a particular variable. So, we create a variable user of type UserDetails as shown below:
user: UserDetails
UserDetails Interface

Interface for UserDetails

# 5. Add method documentation for methods as well as parameters passed (Press /** + enter wherever method documentation needs to be added)
Example:

Method documentation

# 6. Keep method/variable names as informative as possible.
Method Name
Example:

Informative method name
Variable Name
Example:
firstName: string

# 7. Use data access specifiers while declaring variables/methods (Like public/private etc)
Example:
If we declare a variable ‘firstNumber’ and it is used only inside the class say ‘Addition’, it is marked as private.
private firstNumber: number
Similarly, a method can be marked as private if it is only used inside a particular class.
private sumOfTwoNumbers(): number {}
However, If a variable is used in an HTML file, it should be marked public.

# 8. Use TSLint and make sure not to disable any lint rule. TSLint extension should be enabled in order to include lint rules in the project.

# 9. Scope of the variables should be as minimum as possible.
Example:
Since FIRST_NUMBER is used only inside the method sumOfTwoNumber, it is initialised inside that particular method, thus limiting the scope of the variable to that particular method.

Scope of FIRST_NUMBER

# 10. Avoid using repetitive if else (Use switch case instead)
Example:

Switch case

# 11. Use try catch to handle the error and exceptions. Make sure there is no unhandled exception in your code.
Example:

Try catch block for error handling

# 12. Always log the errors and relevant information. This helps in debugging the code in case of errors. The following log levels can be used to add logging in your code:
Error
Example:
console.error('This is an error log')
Warn
Example:
console.warn('This is an warning log')
Info
Example:
console.info('This is an info log')
Debug
Example:
console.debug('This is a debug log')
Trace
Example:
console.trace('This is a trace log')

# 13. Add TODOs for pending code blocks.
Example:

TODO for pending code block
# 14. Reuse the code as much as possible and remove unnecessary code blocks.
