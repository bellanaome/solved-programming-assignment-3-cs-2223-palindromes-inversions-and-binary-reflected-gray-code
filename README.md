Download Link: https://assignmentchef.com/product/solved-programming-assignment-3-cs-2223-palindromes-inversions-and-binary-reflected-gray-code
<br>
<ol>

 <li>(10 Points) A <em>palindrome </em>is a word, phrase, or sequence that reads the same backward as forward. Write a recursive C++ program/procedure which determines whether an input sequence (string) from the keyboard is a palindrome or not. There is no need for fancy classes, etc. here. (You can assume the input will be shorter than 256 characters.)</li>

</ol>

Call your program/project ‘palindromecheck’.

Three Bonus Points: Make your program case insensitive, and have your program ignore white space and punctuation:

“Never odd or even”

“Able was I ere I saw Elba”

“A man, a plan, a canal: Panama!”

<ol start="2">

 <li>(25 Points) Let <em>A</em>[0<em>..n</em>−1] be an array of real numbers (or any ordered set). A pair (<em>A</em>[<em>i</em>]<em>,A</em>[<em>j</em>]) is said to be an <em>inversion </em>if these numbers (elements) are out of order, i.e., <em>i &lt; j </em>but <em>A</em>[<em>i</em>] <em>&gt; A</em>[<em>j</em>]. Note that this pair need not be adjacent. The array/sequence (3, 2, 1) contains <em>three </em>inversions: (3,2), (2,1), and (3,1).</li>

</ol>

(10 Points) Write a program with a na¨ıve <em>O</em>(<em>n</em><sup>2</sup>) algorithm that counts the number of inversions in such an array <em>A</em>. Hint: Bubblesort is <em>O</em>(<em>n</em><sup>2</sup>). Call your program/project ‘easyinversioncount’.

(15 Points) Write a program with a <em>O</em>(<em>n</em>log<em>n</em>) algorithm that counts the number of inversions in such an array <em>A</em>.

Call your program/project ‘fastinversioncount’. (Hint 2 to follow…Wednesday …)

1

<ol start="3">

 <li>(15 Points) Binary Reflected Gray Code</li>

</ol>

Professor Wolfe has four children: Alice, Bob, Chris, and Dylan. Each year for Arbor Day the family goes on a tree-planting picnic, and Professor Wolfe takes photos of the kids in every possible subset arrangement with the new trees they have planted as a backdrop. It’s a lovely tradition. However, last year with newborn Dylan things got more complicated. In transitioning from photograph 7 (0111) to photograph 8 (1000), Professor Wolfe placed baby Dylan on the picnic blanket while all the other children got up and left the scene. Mayhem ensued. Bob and Chris started chasing each other with rakes, and Alice complained about having to move every time a photo was to be taken.

This year is going to be different. Instead of using a binary counting sequence to ensure that all the subset arrangements are made, Professor Wolfe is going to use the Binary Reflected Gray Code of order four. In this way, each transition from one subset of children to the next can be made by having just one child enter or leave the tableau:

<table width="375">

 <tbody>

  <tr>

   <td width="51">Index</td>

   <td width="88">Gray Code</td>

   <td width="157">Child(ren) in Photo</td>

   <td width="80">Action</td>

  </tr>

  <tr>

   <td width="51">1</td>

   <td width="88">0001</td>

   <td width="157">Alice</td>

   <td width="80">Alice In</td>

  </tr>

  <tr>

   <td width="51">2</td>

   <td width="88">0011</td>

   <td width="157">Bob &amp; Alice</td>

   <td width="80">Bob In</td>

  </tr>

  <tr>

   <td width="51">3</td>

   <td width="88">0010</td>

   <td width="157">Bob</td>

   <td width="80">Alice Out</td>

  </tr>

  <tr>

   <td width="51">4</td>

   <td width="88">0110</td>

   <td width="157">Chris &amp; Bob</td>

   <td width="80">Chris In</td>

  </tr>

  <tr>

   <td width="51">5</td>

   <td width="88">0111</td>

   <td width="157">Chris &amp; Bob &amp; Alice</td>

   <td width="80">Alice In</td>

  </tr>

  <tr>

   <td width="51">6</td>

   <td width="88">0101</td>

   <td width="157">Chris &amp; Alice</td>

   <td width="80">Bob Out</td>

  </tr>

  <tr>

   <td width="51">…</td>

   <td width="88">…</td>

   <td width="157">Etc.</td>

   <td width="80">Etc.</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>(5 Points) Using C++, implement algorithm brgc(<em>n</em>) on page 148 of Levitin to produce the Binary Reflected Gray Code of order <em>n</em>.</li>

 <li>(5 Points) Add to your routine (or write a separate one using the idea in Problem 9b on page 149 of Levitin) to create a sequence of names representing which child must move when.</li>

</ul>

The partial sequence up to six is: Alice, Bob, Alice, Chris, Alice, Bob, …

<ul>

 <li>(5 Points) Put it all together to complete the table above for all 15 photos Professor Wolfe wants to take. You can even start at 0=0000, if you like.</li>

</ul>

Call your program/project ‘graycodesarefun’.

Where have we seen this before? How many interesting patterns can <em>you </em>find?

Can you extend your code to Eve? Felix? Gerry? Helen? Ian? Jane? Karl…?