Download Link: https://assignmentchef.com/product/solved-cs2110-timed-lab3-lc-3-assembly
<br>
You are given a string of essentially random characters, and your task is to replace all non-numeric characters with space characters.

<h1><a name="_Toc21715"></a>4           Instructions</h1>

The following files have been provided for you:

<ol>

 <li>timedlab3.asm</li>

</ol>

You will be editing timedlab3.asm to replace instances of non-numeric characters in a string with space characters. The space character (i.e. ‘ ‘) corresponds to decimal value 32 in ASCII. All other ASCII characters in the provided string, outside of the range ‘0’…’9′ should be replaced with ‘ ‘.

<em>Remember: </em>Strings are zero-terminated arrays of characters!

<strong>An ASCII table has been provided for your reference at the end of this document: </strong>The space character is highlighted with red and the numeric digits are highlighted with yellow .

We have defined the following assembly language labels for you:

<ul>

 <li>STR ADDR: The address of the beginning of the string Consider the following examples:</li>

</ul>

<table width="200">

 <tbody>

  <tr>

   <td width="100"><strong>Before</strong></td>

   <td width="100"><strong>After</strong></td>

  </tr>

  <tr>

   <td width="100">“a3hf5k32ss”</td>

   <td width="100">” 3 5 32 “</td>

  </tr>

  <tr>

   <td width="100">“A3HF5K32SS”</td>

   <td width="100">” 3 5 32 “</td>

  </tr>

  <tr>

   <td width="100">“aBcD3fGhIj”</td>

   <td width="100">”          3            “</td>

  </tr>

 </tbody>

</table>

<em>Note: </em>Replace characters in the existing string. Do not copy it!

<em>Hint: </em>You may create your own labels with .fills!

<h2><a name="_Toc21716"></a>4.1         Restrictions</h2>

You are not allowed to use the JSR and JSRR instructions for this assignment. In addition, you are not allowed to use Appendix-A or the textbook during this timed lab.

<h1><a name="_Toc21717"></a>5           Testing Your Work</h1>

To test your program, upload timedlab3.asm to the Timed Lab 3 assignment on Gradescope. You may resubmit your work as many times as needed, until you sign out and leave the classroom.

<h1><a name="_Toc21718"></a>6           Common Errors</h1>

To trace problems with your code, load the file into complx, the LC-3 simulator. To use complx:

<ol>

 <li>In the Terminal, type complx</li>

 <li>In the File menu, click Reload, and open your assembly file (asm)</li>

 <li>Use the Step button to run each instruction one step at a time, or use the Run button to execute all of the instructions until HALT</li>

</ol>

<h1><a name="_Toc21719"></a>7           Rubric</h1>

The output of the Gradescope autograder is an approximation of your score on this assignment. The tool is provided so you can evaluate whether your submission fulfills the assignment expectations.

<em>However</em>, we reserve the right to run additional tests, fewer tests, different tests, or potentially change individual tests – your final score will be determined by your instructors, and there is no guarantee your score will correlate with tester output.

<h1><a name="_Toc21720"></a>8           Deliverables</h1>

Please upload the following files to the assignment on Gradescope:

<ol>

 <li>timedlab3.asm</li>

</ol>

<strong>Do NOT upload an archive, upload the file individually.</strong>

<strong>Be sure to check your Gradescope test score before you leave the room.</strong>

<h1><a name="_Toc21721"></a>9           LC-3 Assembly Programming Requirements</h1>

<h2><a name="_Toc21722"></a>9.1         Overview</h2>

<ol>

 <li>Your code must assemble with <strong>NO WARNINGS OR ERRORS</strong>. To assemble your program, open the file with Complx. It will complain if there are any issues. <strong>If the code in this file does not assemble, you WILL get a zero for that file.</strong></li>

 <li><strong>Comment your code! </strong>This is especially important in assembly, because it’s much harder to interpret what is happening later, and you’ll be glad you left yourself notes on what certain instructions are contributing to the code. Comment things like what registers are being used for and what less intuitive lines of code are actually doing. To comment code in LC-3 assembly just type a semicolon (;), and the rest of that line will be a comment.</li>

 <li>Avoid stating the obvious in your comments; it doesn’t help in understanding what the code is doing. Try to write high-level pseudo-code instead!</li>

</ol>

<strong>Good Comment</strong>

<table width="404">

 <tbody>

  <tr>

   <td width="167">ADD R3, R3, -1</td>

   <td width="237">; counter–</td>

  </tr>

  <tr>

   <td width="167">BRp LOOP<strong>Bad Comment</strong></td>

   <td width="237">; if counter == 0 don’t loop again</td>

  </tr>

  <tr>

   <td width="167">ADD R3, R3, -1</td>

   <td width="237">; Decrement R3</td>

  </tr>

  <tr>

   <td width="167">BRp LOOP</td>

   <td width="237">; Branch to LOOP if positive</td>

  </tr>

 </tbody>

</table>


