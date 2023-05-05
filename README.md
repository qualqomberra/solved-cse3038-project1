Download Link: https://assignmentchef.com/product/solved-cse3038-project1
<br>
In this project, you are required to implement some procedures in MIPS assembly language. You will use SPIM simulator [1] to develop and test your code. There will be three questions in the project which are unrelated.

<strong>QUESTION 1.</strong>  In this program you are required to implement a number series for square root of 2 approximation based on given inputs. Following algorithm used to approximate square root  of 2 by the ancient mathematicians.

<h1> Iteration             <em>a</em> <em>        </em>   <em>b</em> <em>        </em>   <em>a</em><em><sup>2</sup></em>  <em>-2b</em> <em><sup>2</sup></em>    <em>           </em>  <em>a/b</em></h1>

<table width="320">

 <tbody>

  <tr>

   <td width="138">1                      1</td>

   <td width="47">1</td>

   <td width="34">-1</td>

   <td width="100">1</td>

  </tr>

  <tr>

   <td width="138">2                      3</td>

   <td width="47">2</td>

   <td width="34">+1</td>

   <td width="100">1.500</td>

  </tr>

  <tr>

   <td width="138">3                      7</td>

   <td width="47">5</td>

   <td width="34">-1</td>

   <td width="100">1.400</td>

  </tr>

  <tr>

   <td width="138">4                      17</td>

   <td width="47">12</td>

   <td width="34">+1</td>

   <td width="100">1.417</td>

  </tr>

  <tr>

   <td width="138">5                      41</td>

   <td width="47">29</td>

   <td width="34">-1</td>

   <td width="100">1.414</td>

  </tr>

 </tbody>

</table>

<em>a</em><em><sub>2</sub>= a</em><em><sub>1</sub>+2b</em><em><sub>1 </sub>b</em><em>2=a</em><em>1+b</em><em>1</em>

Your program should take a iteration count and print the list of nominator and denominator for approximation. Next iteration <em>a</em> value is calculated by<em> a+2b </em>and next iteration <em>b</em> is calculated by <em>a+b</em>. All the numbers in the series should fit in a word!

An example run:

Enter the number of iteration for the series: 5

a: 1 3 7 17 41 b: 1 2 5 12 29

<strong>QUESTION  2</strong><strong>.</strong><em> (22 points)</em> In this question, you are required to implement matrix

multiplication in MIPS. Given two list of linear arrays and matrices dimensions as inputs, output multiplication matrix will be printed. You can assume that matrix input sizes will always be valid. For example if first matrix in length of <strong><em>mxn</em></strong>, second matrix will be in length of <strong><em>nxk</em></strong>. User will only enter dimensions <strong><em>m </em></strong>and <strong><em>n </em></strong>where you can derive <strong><em>k</em></strong> from length of second matrix<strong><em>.</em></strong> You will assume matrices are given in row and then column order.  For example if matrix elements are:

3 5 4 6 2 8 and dimensions are 3×2, matrix is:

<ul>

 <li>5</li>

 <li>6</li>

 <li>8</li>

</ul>

or if the dimensions are 2×3, matrix is:

<ul>

 <li>5 4</li>

</ul>

6 2 8

An example run:

Enter the first matrix:  3 7 8 12 5 6 7 2 4 3 2 5

Enter the second matrix: 2 5 6 3 7 8 9 1

Enter the first dimension of first matrix: 3

Enter the second dimension of first matrix: 4

Multiplication matrix:

212      112

113      101

85        50

<strong>QUESTION 3.</strong> <em>(</em>Write a MIPS program that performs <u>case insensitive</u> palindrome checker. Given any string with the maximum length of 100 characters, you program will decide if the given string is palindrome or not. Palindrome strings are strings that are equivalent to their reverse. If the lower case letter is matched with the upper case letter in the reverse, it is a valid palindrome.

Examples palindrome strings:

ABBA

Step on no pets abGcdEEedcgba

<u>Example Runs:</u>

Enter an input string: abGcdEEedcgba abgcdeeedcgba is palindrome.

Enter an input string: ABBnMBBa abbnmbba is not palindrome.

<strong>MENU  </strong><em>(8 points): </em>Your program should support a <em>Menu</em> including all questions above. A sample execution scenario given below:

Welcome to our MIPS project!

Main Menu:

1.Square Root Approximate

2.Matrix Multiplication

3.Palindrome

4.Exit

Please select an option: 1

These options must be printed inside a loop until “Exit” option is selected.  When the user select option 1, you should print the followings:

Enter the number of iteration for the series: 5 a: 1 3 7 17 41 b: 1 2 5 12 29

Main Menu:

1.Square Root Approximate

2.Matrix Multiplication

3.Palindrome

4.Exit

Please select an option: 2

Enter the first matrix:  3 7 8 12 5 6 7 2 4 3 2 5

Enter the second matrix: 2 5 6 3 7 8 9 1

Enter the first dimension of first matrix: 3

Enter the second dimension of first matrix: 4

Multiplication matrix:

212 112

113 101

85 50

Main Menu:

1.Square Root Approximate

2.Matrix Multiplication

3.Palindrome

4.Exit

Please select an option: 3 Enter an input string: abGcdEEedcgba abgcdeeedcgba is palindrome. Main Menu:

1.Square Root Approximate

2.Matrix Multiplication

3.Palindrome

4.Exit

Please select an option: 4

Program ends. Bye &#x1f642;