Download Link: https://assignmentchef.com/product/solved-ch-230-a-assignment-13-streams-multiple-inheritance-and-exceptions
<br>
<h1>Problem 13.1 <em>Copy a file                                                                                              </em></h1>

Write a program which reads from the standard input the name of a file (e.g., “input.txt”). Your program should use C++ streams to create a copy of this file with the name as the original file name concatenated with “_copy” and then the original extension (e.g., “input_copy.txt”). <em>You can assume that the input will be valid and the necessary input file has a valid content if existing.</em>

<h2><strong>Problem 13.2 </strong>Complex class with streams                                                                 (</h2>

Adapt and extend your previous source code for working with complex numbers (Complex.h,

Complex.cpp and testComplex.cpp) such that the operators + for adding, – for subtracting, <sup>∗ </sup>for multiplying two complex numbers, = for assigning, &lt;&lt; and &gt;&gt; for input and output streams are overloaded. Your testing program (testComplex.cpp) should read two complex numbers from the files called in1.txt and in2.txt, then compute their sum, the difference and the product, and print the results on the screen as well as into a file called output.txt. You have the freedom to set the structure of the input files.

<em>You can assume that the input of the testing program will be valid and the necessary input files have a valid content if existing.</em>

<h2><strong>Problem 13.3 </strong>Concatenate n files into new file</h2>

Write a program which reads from the standard input an integer value n, followed by n file names. Your program has to concatenate the content of the n files and write the result into the file called “concatn.txt” using binary read and write. Add a ’
’ to separate the contents of the different files inside the resulting file. The operation of the concatenation is successful only if all files are existing and their opening was successful.

<em>You can assume that the input will be valid and the necessary input files have a valid content if existing.</em>

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 13.4 </strong><em>Multiple inheritance I</em></td>

  </tr>

  <tr>

   <td width="457"> </td>

  </tr>

 </tbody>

</table>

Compile and run the file. If you find any compilation errors, explain their reason as comments in the code. Then fix the errors such that the program compiles and runs. Explain the motivation of your modifications in the code and their effects on the execution.

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 13.5 </strong><em>Multiple inheritance II</em></td>

  </tr>

 </tbody>

</table>

Compile and run the file. If you find any compilation errors, explain their reason as comments in the code. Then fix the errors such that the program compiles and runs. Explain the motivation of your modifications in the code and their effects on the execution.

<h2><strong>Problem 13.6 </strong>Out of range exception</h2>

Write a program which creates a vector of integers and adds the value 8, 20 times into the vector.

Include the library &lt;vector&gt; and then create a vector object which stores the 20 values from

th above. Then write a try and catch block in which your code should try to access the 21 element from the vector using the at() method. The exception you should catch should be of type out_of_range. In the catch block use cerr to print to the standard error stream the type of the exception by calling the redefined what() method inherited from the exception class.

<h2><strong>Problem 13.7 </strong>Simple different exceptions</h2>

Write a program and a function with an integer parameter which can throw four exception types: a char, an int, a bool, and your own exception class called OwnException derived from exception. If the parameter of the function is 1 then the character ’a’ should be thrown, if it’s 2 then the integer 12 should be thrown, if it’s 3 then the bool value true should be thrown, and in the default case an OwnException with the string ”Default case exception” should be thrown. You should overwrite the what() method for the OwnException class by returning the string ”OwnException
”. Call the function in the main function in its four versions and catch the corresponding exceptions. In the catch blocks you should print to the standard error stream cerr the string ”Caught in main: ” followed by the value of the thrown exception. In the case of OwnException print the string returned by the what() method.

<h2><strong>Problem 13.8 </strong>Car exceptions</h2>

Write a Garage class that has a Car (i.e., object of a second class) that is having troubles with its Motor (i.e., object of a third class). Use a function-level try block in the Garage class constructor to catch an exception (thrown from the Motor class with the string ”This motor has problems”) when its Car object is initialized. Throw a different exception with the string

”The car in this garage has problems with the motor” from the body of the Garage constructor’s handler and catch it in the main function.