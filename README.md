# String_Calculator_Kata

This repository contains my implementation of a String Calculator which recieves a string (containing zero or more numbers as well as some delimeters) as input and calculates the string's sum based on a number of rules/requirements specified by the project and which can be found later in this README file. Furthermore, it is worth mentioning that this Kata was designed to introduce interns to testing with XUnit.net as well as some of the more advanced testing concepts/techniques/libraries such as: Moq, Test-Driven Development, Behavior Verification, and Outside-In TDD. While not all of these techniques/libraries may be deployed in my implementation of the String Calculator, some were utilized in order to test each of the 6 steps required to complete this project. The techniques employed proved to be invaluable when driving the design of the String Calculator as well as testing this calculator for functionality. All test files can be found in the String_Calculator_Kata.Tests folder of this repository.

As part of my internship as a Backend Development Intern at Foothill Technology Solutions, I was asked to complete a task-based training program. This training program involves taking online courses to better hone and improve an intern's programming skills and work with development teams to get a taste of what a career in software development is like all while performing tasks (doing assigned projects) that help deepen an intern's understanding of the material and the training they are receiving.

For my third task, I was asked to implement a String Calculator console application, using C#, that performs addition of the contents of a provided string (should there be any numbers in the string) within a given set of rules that can be found later in this README file. This exercise is meant to help interns become familiar with what a sofware development process over time might look like, become familiar with C#'s XUnit.net testing library (in addition to more advanced testing techniques such as TDD, Outside-In TDD, Behavior Verification and the Moq library), as well as making interns become more comfortable employing the skills that they learn during their training at the company.

Here is a description of the instructions I received for this project:

Before you start:
Use Console application template.
Write unit tests for each requirement.
Try not to read ahead.
Do one task at a time. The trick is to learn to work incrementally.
Make sure you only test for correct inputs. There is no need to test for invalid inputs for this kata.
Follow GIT best practices you learned to push your code, and push each task into separate commits.

The kata:
Step 1: the simplest thing
  Create a simple String calculator with a method int add(String numbers).
  The string argument can contain 0, 1 or 2 numbers, and will return their sum (for an empty string it will return 0) for example "" or "1" or "1,2".
  Start with the simplest test case of an empty string and move to 1 and two numbers.
  Remember to solve things as simply as possible so that you force yourself to write tests you did not think about.
  Remember to refactor after each passing test.
  
Step 2: handle an unknown amount of numbers
  Allow the add() method to handle an unknown amount of numbers.
  
Step 3: handle new lines between numbers
  Allow the `add()` method to handle new lines between numbers (instead of commas).
  The following input is ok: "1\n2,3" (will equal 6)
  The following input is NOT ok: "1,\n" (not need to prove it - just clarifying)
  
Step 4: support different delimiters
  Support different delimiters: to change a delimiter, the beginning of the string will contain a separate line that looks like this: "//[delimiter]\n[numbers...]"
  For example `"//;\n1;2"` should return 3 where the default delimiter is `';'`. The first line is optional. All existing scenarios should still be supported.
  
Step 5: negative numbers
  Calling add() with a negative number will throw an exception "negatives not allowed" - and the negative that was passed.
  If there are multiple negatives, show all of them in the exception message.
  
Step 6: ignore big numbers
  Numbers bigger than 1000 should be ignored, so adding 2 + 1001 = 2
  


My implementation of the String Calculator can be found in the String_Calculator_Kata.Classes folder and testing can be found in the String_Calculator_Kata.Tests folder.

Please note that due to the nature of this Kata, some new requirements might replace or break earlier requirements (as the customer might want to override some older features with newer ones). Therefore, by the time you are viewing my solutions, some of the older tasks may not exist anymore. Nonetheless, feel free to fork this project and use Git to move back in history and checkout how this project have progressed over time.

Thanks,

Ayham R.
