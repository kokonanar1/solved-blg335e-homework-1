Download Link: https://assignmentchef.com/product/solved-blg335e-homework-1
<br>
<h1>Homework Policy</h1>

<ul>

 <li>Do not forget to handle exceptions and print error messages!</li>

 <li>Your code must be written in C++, and should be able to be compiled and run using g++ compiler. ITU servers provide g++ compiler, you can test your program by connecting to the servers using ssh(If you don’t know how to do it, <a href="http://www.eskibidb.itu.edu.tr/?d=165">click here</a><a href="http://www.eskibidb.itu.edu.tr/?d=165">)</a>. Using object oriented approach is a bonus. You can not use external libraries such as STL.</li>

</ul>

<h1>Problem Description</h1>

In this project, you are expected to implement Bubble Sort and Merge Sort. You are also required to prepare a report including their analyses and a solution to the given question below.

<h1>Implementation Details(40 Points)</h1>

Two input files (sorted.txt and unsorted.txt) that includes integers to be sorted is provided. Read N numbers from the input file, sort them using Bubble Sort or Merge Sort and report the time that the algorithm takes to sort. You should refer to the lecture materials for Merge Sort algorithm. Additionally, pseudo code for Bubble Sort on an array of numbers <strong>A </strong>is given as follows:

i &lt;- length[A] sorted &lt;- False <strong>while </strong>i is greater than 1 <strong>AND </strong>sorted <strong>is </strong>False sorted &lt;- True

<strong>do for </strong>j &lt;- 1 <strong>to </strong>i – 1 <strong>do if </strong>A[j] &lt; A[j – 1] <strong>then </strong>exchange A[j] &lt;-&gt; A[j – 1] <strong>and </strong>sorted &lt;- False

i &lt;- i-1

Your program should be run from the command line with the following format:

./program algorithmType N file

<strong>N: </strong>Total number of integers to be sorted <strong>algorithmType: </strong>Method to be used to sort( ’b’ for Bubblesort or ’m’ for Merge Sort) <strong>file: </strong>Input file to be read (“sorted.txt” or “unsorted.txt”).

An example execution command is given as follows:

./program m 1000 sorted.txt

This command executes the program using Merge sort with the first 1000 elements of the file “sorted.txt”.

After the execution of your program, an output file should be created (output.txt) with the sorted integers in ascending order and your program should report the time used for the algorithm.

Figure 1: An example table. This is similar to the ones used in the lectures, create a similar one for yourself and use it for asymptotic bound analysis questions below.

<h1>Report(60 points)</h1>

In your report, you are expected to analyze and compare the running times of algorithms you implemented with respect to their computational complexity. In addition, you are going to analyze the time complexity of the ’Mystery’ function given below as well. Therefore, you need to complete the following tasks and include the results in your report.

<ul>

 <li><strong>10 points </strong>Give the asymptotic lower bound <strong>AND </strong>upper bound on the running time for Bubble Sort and Merge Sort with the methods you covered in the lectures using the table above and show that your implementation of these algorithms fit these values.</li>

 <li><strong>10 points </strong>Run each search methods for each different value of <strong>N </strong>as1000, 10000, 100000,1000000 with both of the given input files “sorted.txt” and “unsorted.txt”. Calculate the average time of execution for each value of <strong>N </strong>for each file. <strong>Note: </strong>You can use the <strong>clock() </strong>function under <strong>ctime </strong>library to calculate time of execution for the sort functions. <a href="http://www.cplusplus.com/reference/clibrary/ctime/clock">Click here</a> for more details.</li>

 <li><strong>20 points </strong>After calculating execution times for both of the files, you will prepare two line plots (in Excel or Matlab) for each file, in order to visualize the runtime complexity of Bubble Sort and Merge Sort for different values of <strong>N</strong>. Then you are expected to interpret the results with respect to the asymptotic bounds you have given in <strong>a</strong>. Indicate in which cases you would choose which algorithm. Why?</li>

 <li><strong>20 points </strong>Examine the following <strong>Mystery </strong>function:

  <ol>

   <li>Algorithm Mystery(n)</li>

   <li>r &lt;- 0</li>

   <li>for i &lt;- 1 to n do</li>

   <li>for j &lt;- i+1 to n do</li>

   <li>for k &lt;- 1 to j do</li>

   <li>r &lt;- r+1;</li>

   <li>return r</li>

  </ol></li>

</ul>

What value is returned by the algorithm? Express your answer as a function of n. Compute its time complexity with the same method you used in <strong>a</strong>.

<h1>Submission</h1>

Submit your homework files through Ninova. Please zip and upload all your files. You are going to submit the following files:

<ul>

 <li>All your .h and .cpp files</li>

 <li>a .pdf file as your report. Your report should be clear and detailed. If your solutions are unclear, it may result in a grade loss for you.</li>

 <li>a .txt file explaining how to compile and run your code (in a 1 or 2 line)</li>

</ul>