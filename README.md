Download Link: https://assignmentchef.com/product/solved-cs590-homework4-dynamic-programming-greedy-algorithms
<br>
<pre>The class random—generator has been updated (random—generator.h and ran- dom_generator.cc) by a member function which generates random strings of a fixed length using the a given number of characters from the alphabet, starting with • char* random-string-m(int n, int no-ch) The function allocates n + I characters. The first n characters n — l) are chosen at random using the first no_ch characters from the alphabet start- ing with "a" (e.g., for no-ch = 4 the characters are randomly chosen out of { a , b , The n-th character is set to O in order to mark the end of the string. Dynamic programming (70 points) The dynamic programming Smith-Waterman algorithm is matching sequences recur- sively defined as follows, given X = , , (along table rows) and Y = , ... , ym (along table columns). = 0, for all 0 &lt; i &lt; n , • = 0, for all 0 S j S m — I) + 2 if = Yj = max , — I if is inserted into Y MO-I J) is inserted into X</pre>

<pre><img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/604.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/604.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript></pre>

<pre>The function M (i, j) defines a so called matching score for the partial sequencxs X, and Yj. If in the recursive definition of M the maximum value is due to the third or fourth line, you have to insert the character into either X or Y in order to reconstruct the matching sequences and Y'. Similar to the LCS problem we need only need a table to store the M (i, j) values, but an additional table that allows us to later generate X' and Y' from X and Y. Exam le 3 cdbaabbd ca c-dba--abbd ca cadcacca-bd cadcaccabd 5 x Exam le i abababda a-bababda acbabab-a acbababa 12 Exam le 4 caacbdacca caacb-dacc-a c—— cbcd—ccba bccbcd ccba 9 Exam le 2 cacacccbab ca-cacccbab cadaadcc- bccadaadcc 4 Exarn le 5 dcacccbbba dcacccb-bba d ca —bad ba aad cabadba 7 <img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/472.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/472.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript></pre>

<pre>l. Implement the bottom-up version of the Smith-Waterman algorithm given by the recursive definition of the function M (as seen on the slides). 2. Implement the top-down with memoization version of the Smith-Waterman algorithm given by the recursive definition of the function M. Notes: How do you initialize the necessary tables given the definition of M. Keep in mind that you have to able to determine whether or not you already computed a table value (memoization). Values could be negative, but is there a limit for how small they can get? 3. Implement the function void ) that takes a number of parameters and then recursively prints the matching sequence that is derived from X. Implement a separate function void ... ) that recursively prints the matching sequence that is derived from Y. 4. Find the maximum alignment for X = dcdcbacbbb and Y = acdccabdbb by using the Smith-Waterman algorithm (see slides). Execute the pseudocode algorithm and fill the necessary tables I-I and P in a bottom-up fassion. Re- construct the strings X' and Y' using the tables H and P. (7+20+8+15 50 points) <img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/179.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/179.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript></pre>

<pre>Exercise 15.1-2 Show, by means of a counterexample, that the following greedy" strategy does not always determine an optimal way to cut rods. Define the density of a rod of length i to be that is, its value per inch. The greedy strategy for a rod of length n cuts off a first piece of length i, where 1 i n, having maximum density. It then continues by applying the greedy strategy to the remaining piece of length (7 points) Exercise 15.1-5 The Fibonacci numbers are defines by recurrence (3.22). Give an O(n) time dynamic-programming algorithm to compute the n-th Fibonacci number. Draw the subproblem graph. How many vertices and edges are in the graph? (8 points) Exercise 15.4-1 Determine (0, 1, o, 1, 1,0, 1, 1,0). (5 points) an LCS of and <img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/132.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/04/132.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript></pre>