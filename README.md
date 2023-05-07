Download Link: https://assignmentchef.com/product/solved-kit205-week-2-tutorial
<br>
<h1>Creating a new project</h1>

We will be using Microsoft Visual Studio in this unit.  You should follow the instructions below when creating a new project.

<ol>

 <li>Start Microsoft Visual Studio.</li>

 <li>Choose <em>New Project…</em> from the <em>File</em></li>

 <li>Select the <em>Visual C++</em> template and choose <em>Win32 Console Application</em>.</li>

 <li>Enter a name for the project (e.g. <em>Week2</em>) and check the location at the bottom of the <em>New Project</em> window (you probably want to put it on your network drive in a folder for KIT205). Click <em>OK</em>.</li>

 <li>When the <em>Win32 Application Wizard</em> starts hit the <em>Next&gt;</em></li>

 <li>Choose <em>Empty Project</em> and uncheck <em>Security Development Lifecycle (SDL)</em>, and click</li>

</ol>

<em>Finish</em>.

<ol start="7">

 <li>From the <em>Project</em> menu, choose <em>Add New Item… </em></li>

 <li>Choose a new <em>C++ File</em> and give it a name (e.g. <em>c</em>). Make sure that you change the filename extension from <em>.cpp</em> to <em>.c</em>.</li>

 <li>The new empty file should now be open. Write a simple program (that is, a <em>main</em> method) that displays “hello world” on the console.</li>

 <li>Run the program without debugging (<em>Ctrl F5</em>) so that the console window isn’t immediately closed.</li>

</ol>

<h1>Creating and Testing a Linked List</h1>

<table width="170">

 <tbody>

  <tr>

   <td width="170">•  You will need to  #include &lt;stdlib.h&gt;  to be able to use NULL•  <em>If you declare your list as: List my_list = new_list(); you will need to pass &amp;my_list as the first parameter to the other list functions </em>•  <em>Depending on your project settings, you may need to use scanf_s, instead of scanf (check online for more info) </em></td>

  </tr>

 </tbody>

</table>

Next we are going to get a linked list up and running.  You may find some of the instructions a little light on detail; that is deliberate.  If you need extra help, ask your tutor – but try and work it out for yourself first. J

<ol start="11">

 <li>Add the linked list code from the lectures. The <em>struct</em>, <em>typedef</em> and function prototypes should go in a new header file called <em>h</em> and the function implementations should go in a new source file called <em>list.c</em>.</li>

 <li>Test the linked list by modifying your main function so that it creates a list by adding some ints (<em>insert_at_front</em>) and then printing the list (<em>print_list</em>).</li>

 <li>Test the other functions (<em>insert_in_order</em>, <em>delete_from_list</em>, <em>destroy</em>) as well.</li>

</ol>

<strong> </strong>

<h1>Testing Infrastructure</h1>

In this unit we will be doing a lot of console-based testing.  The following steps will make a start on setting up some testing code (either comment your existing code, or create a new project before continuing).

<ol start="14">

 <li>Modify your main function (e.g. <em>c</em>) so that you:

  <ol>

   <li>Create a List</li>

   <li>Declare an int for storing input</li>

   <li>scanf into the int</li>

   <li>start a while loop that continues until your int has the value 0</li>

   <li>inside the while loop

    <ol>

     <li>add the int to your list</li>

     <li>scanf a new int</li>

    </ol></li>

   <li>destroy the list</li>

  </ol></li>

 <li>Test the above version</li>

 <li>Now modify your main to use a simple menu for selecting functions. The new main should:

  <ol>

   <li>Create a List called <em>my_list</em></li>

   <li>Create an int called <em>quit</em> to that tells the program when to stop and give it the value 0 (false)</li>

   <li>Start a while loop that exits if <em>quit</em> is true (<em>while (!quit){}</em>)</li>

   <li>inside the while loop

    <ol>

     <li>Create an int called <em>option</em></li>

     <li>Print a prompt and scanf into <em>option</em></li>

    </ol></li>

  </ol></li>

</ol>

<ul>

 <li>if <em>option</em> has the value 0, set <em>quit</em> to 1 iv. if <em>option</em> has the value 1, call a new function called <em>option_insert(&amp;my_list)</em></li>

</ul>

<ol>

 <li>if <em>option</em> has the value 2, call a new function called <em>option_delete(&amp;my_list)</em></li>

 <li>if <em>option</em> has the value 3, call a new function called <em>option_print(&amp;my_list)</em></li>

</ol>

<ol>

 <li>destroy the list</li>

</ol>

<ol start="17">

 <li>Create the <em>option_insert</em>, <em>option_delete</em>,and <em>option_print</em> in the same file as main and add/copy code to manipulate the list using your list functions (e.g.</li>

</ol>

<em>option_insert</em> will read an int and then call <em>insert_at_front</em>)

<ol start="18">

 <li>Test the new version</li>

</ol>

<h1>If you have time…</h1>

<ol start="19">

 <li>Add a list function called <em>reverse</em> that takes a list and returns a new list that is the reverse of the given list</li>

 <li>Add a list function called <em>merge</em> that takes two ordered lists as parameters and creates a merged list that is also ordered</li>

 <li>See if you can do it without using <em>insert_in_order</em> or nested loops</li>

</ol>


