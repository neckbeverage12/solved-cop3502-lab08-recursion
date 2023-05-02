Download Link: https://assignmentchef.com/product/solved-cop3502-lab08-recursion
<br>
<span style="font-size: 2.61792em; letter-spacing: -1px;">Overview</span>

This lab is designed to illustrate concepts and characteristics of recursion, including the difference between “regular recursion” and “tail recursion,” the use of base cases, the concept of the call stack, and arithmetic in return statements. You will write three different public methods and a private helper method in this lab. You must strictly follow the given method signatures and specifications.




<h1>Specification</h1>

You create a Factorial class which will implement several versions of a factorial calculation. The recursive definition for factorial is as follows:




Base Case:                                    factorial(1) = 1

Recurrence Relation:                          factorial(n) = n * factorial(n – 1)




<u>The factorial function is undefined for non-positive numbers (including zero)</u>; if a non-positive number is passed in, the function should throw an IllegalArgumentException.




The Factorial class should have the following methods:




public static long pureRecursive(int n)

A purely recursive function that calculates the factorial of n. This function should call <u>only itself</u>.




public static long tailRecursive(int n)

A kickoff method for tail recursion; it should call only the tail() method (see below).




private static long tail(…)

A private method called by the tail recursion kickoff method. Students may select the parameters for this method, but it must be present and used. This method should only call itself, and only via tail recursion – i.e., <u>it</u> <u>should call itself on the last line with no other computation after the function call</u>.




public static long iterative(int n)

An iterative version of the factorial calculation. This method should be an “unwound” version of the tailRecursive() method outlined above. It should not call itself or any other method but should instead using a looping structure to calculate the factorial.










<h1>Submissions</h1>

NOTE: Your output must match the example output *exactly*. If it does not, you will not receive full credit for your submission!




Files:               Factorial.java

Method: Submit on Canvas

<h1>Sample Results (Public Methods)</h1>




<table width="338">

 <tbody>

  <tr>

   <td width="66">Param.</td>

   <td width="272">Returns</td>

  </tr>

  <tr>

   <td width="66">0</td>

   <td width="272">throws IllegalArgumentException</td>

  </tr>

  <tr>

   <td width="66">1</td>

   <td width="272">1</td>

  </tr>

  <tr>

   <td width="66">2</td>

   <td width="272">2</td>

  </tr>

  <tr>

   <td width="66">3</td>

   <td width="272">6</td>

  </tr>

  <tr>

   <td width="66">4</td>

   <td width="272">24</td>

  </tr>

  <tr>

   <td width="66">5</td>

   <td width="272">120</td>

  </tr>

  <tr>

   <td width="66">6</td>

   <td width="272">720</td>

  </tr>

  <tr>

   <td width="66">7</td>

   <td width="272">5,040</td>

  </tr>

  <tr>

   <td width="66">8</td>

   <td width="272">40,320</td>

  </tr>

  <tr>

   <td width="66">9</td>

   <td width="272">362,880</td>

  </tr>

  <tr>

   <td width="66">10</td>

   <td width="272">3,628,800</td>

  </tr>

  <tr>

   <td width="66">11</td>

   <td width="272">39,916,800</td>

  </tr>

  <tr>

   <td width="66">12</td>

   <td width="272">479,001,600</td>

  </tr>

  <tr>

   <td width="66">13</td>

   <td width="272">6,227,020,800</td>

  </tr>

  <tr>

   <td width="66">14</td>

   <td width="272">121,645,100,408,832,000</td>

  </tr>

  <tr>

   <td width="66">15</td>

   <td width="272">2,432,902,008,176,640,000</td>

  </tr>

 </tbody>

</table>


