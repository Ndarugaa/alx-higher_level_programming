# 0x00. Python - Hello, World

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="https://docs.python.org/3/tutorial/index.html" title="The Python tutorial" target="_blank">The Python tutorial</a> (<em>only the first three chapters below</em>)</li>
<li><a href="https://docs.python.org/3/tutorial/appetite.html" title="Whetting Your Appetite" target="_blank">Whetting Your Appetite</a> </li>
<li><a href="https://docs.python.org/3/tutorial/interpreter.html" title="Using the Python Interpreter" target="_blank">Using the Python Interpreter</a> </li>
<li><a href="https://docs.python.org/3/tutorial/introduction.html" title="An Informal Introduction to Python" target="_blank">An Informal Introduction to Python</a> (<em>Read up until &ldquo;3.1.2. Strings&rdquo; included</em>)</li>
<li><a href="https://realpython.com/python-f-strings/" title="How To Use String Formatters in Python 3" target="_blank">How To Use String Formatters in Python 3</a> </li>
<li><a href="https://www.youtube.com/playlist?list=PLGLfVvz_LVvTn3cK5e6LjhgGiSeVlIRwt" title="Learn to Program" target="_blank">Learn to Program</a> </li>
<li><a href="https://pypi.org/project/pycodestyle/" title="Pycodestyle -- Style Guide for Python Code" target="_blank">Pycodestyle &ndash; Style Guide for Python Code</a> </li>
</ul>

<h2>Learning Objectives</h2>

<h3>General</h3>

<ul>
<li>Why Python programming is awesome</li>
<li>Who created Python</li>
<li>Who is Guido van Rossum</li>
<li>Where does the name &lsquo;Python&rsquo; come from</li>
<li>What is the Zen of Python</li>
<li>How to use the Python interpreter</li>
<li>How to print text and variables using <code>print</code></li>
<li>How to use strings</li>
<li>What are indexing and slicing in Python</li>
<li>What is the official Python coding style and how to check your code with <code>pycodestyle</code></li>
</ul>

<h2>Requirements</h2>

<h3>Python Scripts</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)</li>
<li>All your files should end with a new line</li>
<li>The first line of all your files should be exactly <code>#!/usr/bin/python3</code></li>
<li>A <code>README.md</code> file at the root of the repo, containing a description of the repository</li>
<li>A <code>README.md</code> file, at the root of the folder of <em>this</em> project, is mandatory</li>
<li>Your code should use the pycodestyle (version <code>2.8.*</code>)</li>
<li>All your files must be executable</li>
<li>The length of your files will be tested using <code>wc</code></li>
</ul>

<h3>Shell Scripts</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your scripts will be tested on Ubuntu 20.04 LTS</li>
<li>All your scripts should be exactly two lines long (<code>wc -l file</code> should print 2)</li>
<li>All your files should end with a new line</li>
<li>The first line of all your files should be exactly <code>#!/bin/bash</code></li>
<li>All your files must be executable</li>
</ul>

<h3>C Scripts</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89</li>
<li>All your files should end with a new line</li>
<li>Your code should use the <code>Betty</code> style. It will be checked using <a href="https://github.com/alx-tools/Betty/blob/master/betty-style.pl" title="betty-style.pl" target="_blank">betty-style.pl</a> and <a href="https://github.com/alx-tools/Betty/blob/master/betty-doc.pl" title="betty-doc.pl" target="_blank">betty-doc.pl</a></li>
<li>You are not allowed to use global variables</li>
<li>No more than 5 functions per file</li>
<li>In the following examples, the <code>main.c</code> files are shown as examples. You can use them to test your functions, but you don&rsquo;t have to push them to your repo (if you do we won&rsquo;t take them into account). We will use our own <code>main.c</code> files at compilation. Our <code>main.c</code> files might be different from the one shown in the examples</li>
<li>The prototypes of all your functions should be included in your header file called <code>lists.h</code></li>
<li>Don’t forget to push your header file</li>
<li>All your header files should be include guarded</li>
</ul>

<h2>More Info</h2>

<h3>Pycodestyle</h3>

<p><code>Pycodestyle</code> is now the <a href="https://github.com/PyCQA/pycodestyle/wiki" title="new standard of Python style code" target="_blank">new standard of Python style code</a></p>

<p><br />
<br />
<img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/231/Flyingcircus_2.jpg" alt="" loading='lazy' style="" /></p>

  </div>
</div>

<h1>Tasks</h1>
<br>

<h3>0. Run Python file</h3>
<p>Write a Shell script that runs a Python script.</p>

<p>The Python file name will be saved in the environment variable <code>$PYFILE</code></p>

<pre><code>frank@ubuntu:~/py/0x00$ cat main.py 
#!/usr/bin/python3
print(&quot;Best School&quot;)

frank@ubuntu:~/py/0x00$ export PYFILE=main.py
frank@ubuntu:~/py/0x00$ ./0-run
Best School
frank@ubuntu:~/py/0x00$ 
</code></pre>

<h3>1. Run inline</h3>
<p>Write a Shell script that runs Python code.</p>

<p>The Python code will be saved in the environment variable <code>$PYCODE</code></p>

<pre><code>frank@ubuntu:~/py/0x00$ export PYCODE=&#39;print(f&quot;Best School: {88+10}&quot;)&#39;
frank@ubuntu:~/py/0x00$ ./1-run_inline 
Best School: 98
frank@ubuntu:~/py/0x00$ 
</code></pre>

 <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      2. Hello, print
    </h3>
<p>Write a Python script that prints exactly <code>&quot;Programming is like building a multilingual puzzle</code>, followed by a new line.</p>

<ul>
<li>Use the function <code>print</code></li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./2-print.py 
&quot;Programming is like building a multilingual puzzle
frank@ubuntu:~/py/0x00$
</code></pre>

<h3 class="panel-title">3. Print integer</h3>

>Complete this <a href="https://github.com/alx-tools/0x00.py/blob/master/3-print_number.py" title="source code" target="_blank">source code</a> in order to print the integer stored in the variable <code>number</code>, followed by <code>Battery street</code>, followed by a new line.</p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/3-print_number.py" title="here" target="_blank">here</a></li>
<li>The output of the script should be:

<ul>
<li>the number, followed by <code>Battery street</code>,</li>
<li>followed by a new line</li>
</ul></li>
<li>You are not allowed to cast the variable <code>number</code> into a string</li>
<li>Your code must be 3 lines long</li>
<li>You have to use f-strings <a href="https://realpython.com/python-f-strings/" title="tips" target="_blank">tips</a></li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./3-print_number.py
98 Battery street
frank@ubuntu:~/py/0x00$ 
</code></pre>

<h3>4. Print float</h3>


<p>Complete the source code in order to print the float stored in the variable <code>number</code> with a precision of 2 digits.</p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/4-print_float.py" title="here" target="_blank">here</a></li>
<li>The output of the program should be:

<ul>
<li><code>Float:</code>, followed by the float with only 2 digits</li>
<li>followed by a new line</li>
</ul></li>
<li>You are not allowed to cast <code>number</code> to string</li>
<li>You have to use f-strings</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./4-print_float.py
Float: 3.14
frank@ubuntu:~/py/0x00$ 
</code></pre>

<p>Complete this <a href="https://github.com/alx-tools/0x00.py/blob/master/5-print_string.py" title="source code" target="_blank">source code</a> in order to print 3 times a string stored in the variable <code>str</code>, followed by its first 9 characters.</p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/5-print_string.py" title="here" target="_blank">here</a></li>
<li>The output of the program should be:

<ul>
<li>3 times the value of <code>str</code></li>
<li>followed by a new line</li>
<li>followed by the 9 first characters of <code>str</code></li>
<li>followed by a new line</li>
</ul></li>
<li>You are not allowed to use any loops or conditional statement</li>
<li>Your program should be maximum 5 lines long</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./5-print_string.py 
Holberton SchoolHolberton SchoolHolberton School
Holberton
frank@ubuntu:~/py/0x00$ 
</code></pre>

<p>Complete this <a href="https://github.com/alx-tools/0x00.py/blob/master/6-concat.py" title="source code" target="_blank">source code</a> to print <code>Welcome to Holberton School!</code></p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/6-concat.py" title="here" target="_blank">here</a></li>
<li>You are not allowed to use any loops or conditional statements.</li>
<li>You have to use the variables <code>str1</code> and <code>str2</code> in your new line of code</li>
<li>Your program should be exactly 5 lines long</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./6-concat.py
Welcome to Holberton School!
frank@ubuntu:~/py/0x00$ wc -l 6-concat.py
5 6-concat.py
frank@ubuntu:~/py/0x00$ 
</code></pre>

<p>Complete this <a href="https://github.com/alx-tools/0x00.py/blob/master/7-edges.py" title="source code" target="_blank">source code</a></p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/7-edges.py" title="here" target="_blank">here</a></li>
<li>You are not allowed to use any loops or conditional statements</li>
<li>Your program should be exactly 8 lines long</li>
<li><code>word_first_3</code> should contain the first 3 letters of the variable <code>word</code></li>
<li><code>word_last_2</code> should contain the last 2 letters of the variable <code>word</code></li>
<li><code>middle_word</code> should contain the value of the variable <code>word</code> without the first and last letters</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./7-edges.py
First 3 letters: Hol
Last 2 letters: on
Middle word: olberto
frank@ubuntu:~/py/0x00$ wc -l 7-edges.py
8 7-edges.py
frank@ubuntu:~/py/0x00$ 
</code></pre>

<p>Complete this <a href="https://github.com/alx-tools/0x00.py/blob/master/8-concat_edges.py" title="source code" target="_blank">source code</a> to print <code>object-oriented programming with Python</code>, followed by a new line.</p>

<ul>
<li>You can find the source code <a href="https://github.com/alx-tools/0x00.py/blob/master/8-concat_edges.py" title="here" target="_blank">here</a></li>
<li>You are not allowed to use any loops or conditional statements</li>
<li>Your program should be exactly 5 lines long</li>
<li>You are not allowed to create new variables</li>
<li>You are not allowed to use string literals</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./8-concat_edges.py
object-oriented programming with Python
frank@ubuntu:~/py/0x00$ wc -l 8-concat_edges.py
5 8-concat_edges.py
frank@ubuntu:~/py/0x00$ 
</code></pre>

<h3>9. Easter Egg</h3>

<p>Write a Python script that prints &ldquo;The Zen of Python&rdquo;, by TimPeters, followed by a new line.</p>

<ul>
<li>Your script should be maximum 98 characters long (please check with <code>wc -m 9-easter_egg.py</code>)</li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./9-easter_egg.py
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren&#39;t special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you&#39;re Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it&#39;s a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let&#39;s do more of those!
frank@ubuntu:~/py/0x00$
</code></pre>

<p><strong>Technical interview preparation</strong>: </p>

<ul>
<li>You are not allowed to google anything</li>
<li>Whiteboard first</li>
<li>This task and all future technical interview prep tasks will include checks for the efficiency of your solution, i.e. is your solution&rsquo;s runtime fast enough, does your solution require extra memory usage / mallocs, etc.</li>
</ul>

<p>Write a function in C that checks if a singly linked list has a cycle in it.</p>

<ul>
<li>Prototype: <code>int check_cycle(listint_t *list);</code></li>
<li>Return: <code>0</code> if there is no cycle, <code>1</code> if there is a cycle</li>
</ul>

<p>Requirements:</p>

<ul>
<li>Only these functions are allowed: <code>write</code>, <code>printf</code>, <code>putchar</code>, <code>puts</code>, <code>malloc</code>, <code>free</code></li>
</ul>

<pre><code>carrie@ubuntu:~/0x00$ cat lists.h
#ifndef LISTS_H
#define LISTS_H

#include &lt;stdlib.h&gt;

/**
 * struct listint_s - singly linked list
 * @n: integer
 * @next: points to the next node
 *
 * Description: singly linked list node structure
 * 
 */
typedef struct listint_s
{
    int n;
    struct listint_s *next;
} listint_t;

size_t print_listint(const listint_t *h);
listint_t *add_nodeint(listint_t **head, const int n);
void free_listint(listint_t *head);
int check_cycle(listint_t *list);

#endif /* LISTS_H */
</code></pre>

<pre><code>carrie@ubuntu:~/0x00$ cat 10-linked_lists.c
#include &lt;stdio.h&gt;
#include &lt;stdlib.h&gt;
#include &quot;lists.h&quot;

/**
 * print_listint - prints all elements of a listint_t list
 * @h: pointer to head of list
 * Return: number of nodes
 */
size_t print_listint(const listint_t *h)
{
    const listint_t *current;
    unsigned int n; /* number of nodes */

    current = h;
    n = 0;
    while (current != NULL)
    {
        printf(&quot;%i\n&quot;, current-&gt;n);
        current = current-&gt;next;
        n++;
    }

    return (n);
}

/**
 * add_nodeint - adds a new node at the beginning of a listint_t list
 * @head: pointer to a pointer of the start of the list
 * @n: integer to be included in node
 * Return: address of the new element or NULL if it fails
 */
listint_t *add_nodeint(listint_t **head, const int n)
{
    listint_t *new;

    new = malloc(sizeof(listint_t));
    if (new == NULL)
        return (NULL);

    new-&gt;n = n;
    new-&gt;next = *head;
    *head = new;

    return (new);
}

/**
 * free_listint - frees a listint_t list
 * @head: pointer to list to be freed
 * Return: void
 */
void free_listint(listint_t *head)
{
    listint_t *current;

    while (head != NULL)
    {
        current = head;
        head = head-&gt;next;
        free(current);
    }
}
</code></pre>

<pre><code>carrie@ubuntu:~/0x00$ cat 10-main.c
#include &lt;stdlib.h&gt;
#include &lt;string.h&gt;
#include &lt;stdio.h&gt;
#include &quot;lists.h&quot;

/**
 * main - check the code
 *
 * Return: Always 0.
 */
int main(void)
{
    listint_t *head;
    listint_t *current;
    listint_t *temp;
    int i;

    head = NULL;
    add_nodeint(&amp;head, 0);
    add_nodeint(&amp;head, 1);
    add_nodeint(&amp;head, 2);
    add_nodeint(&amp;head, 3);
    add_nodeint(&amp;head, 4);
    add_nodeint(&amp;head, 98);
    add_nodeint(&amp;head, 402);
    add_nodeint(&amp;head, 1024);
    print_listint(head);

    if (check_cycle(head) == 0)
        printf(&quot;Linked list has no cycle\n&quot;);
    else if (check_cycle(head) == 1)
        printf(&quot;Linked list has a cycle\n&quot;);

    current = head;
    for (i = 0; i &lt; 4; i++)
        current = current-&gt;next;
    temp = current-&gt;next;
    current-&gt;next = head;

    if (check_cycle(head) == 0)
        printf(&quot;Linked list has no cycle\n&quot;);
    else if (check_cycle(head) == 1)
        printf(&quot;Linked list has a cycle\n&quot;);

    current = head;
    for (i = 0; i &lt; 4; i++)
        current = current-&gt;next;
    current-&gt;next = temp;

    free_listint(head);

    return (0);
}
</code></pre>

<pre><code>carrie@ubuntu:~/0x00$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 10-main.c 10-check_cycle.c 10-linked_lists.c -o cycle
carrie@ubuntu:~/0x00$$ ./cycle 
1024
402
98
4
3
2
1
0
Linked list has no cycle
Linked list has a cycle
carrie@ubuntu:~/0x00$
</code></pre>

<blockquote>
<p>Solving a problem is already a big win! but finding the best and optimal way to solve it, it&rsquo;s way better! Think about the most optimal / fastest way to do it.</p>
</blockquote>


<h3>11. Hello, write</h3>
<p>Write a Python script that prints exactly <code>and that piece of art is useful - Dora Korpar, 2015-10-19</code>, followed by a new line.</p>

<ul>
<li>Use the function <code>write</code> from the <code>sys</code> module</li>
<li>You are not allowed to use <code>print</code></li>
<li>Your script should print to <code>stderr</code></li>
<li>Your script should exit with the status code <code>1</code></li>
</ul>

<pre><code>frank@ubuntu:~/py/0x00$ ./100-write.py
and that piece of art is useful - Dora Korpar, 2015-10-19
frank@ubuntu:~/py/0x00$ echo $?
1
frank@ubuntu:~/py/0x00$ ./100-write.py 2&gt; q
frank@ubuntu:~/py/0x00$ cat q
and that piece of art is useful - Dora Korpar, 2015-10-19
frank@ubuntu:~/py/0x00$ 
</code></pre>


<h3>12. Compile</h3>
<p>Write a script that compiles a Python script file.</p>

<p>The Python file name will be stored in the environment variable <code>$PYFILE</code></p>

<p>The output filename has to be <code>$PYFILEc</code> (ex: <code>export PYFILE=my_main.py</code> =&gt; output filename: <code>my_main.pyc</code>)</p>

<pre><code>frank@ubuntu:~/py/0x00$ cat main.py 
#!/usr/bin/python3
print(&quot;Best School&quot;)

frank@ubuntu:~/py/0x00$ export PYFILE=main.py
frank@ubuntu:~/py/0x00$ ./101-compile
Compiling main.py ...
frank@ubuntu:~/py/0x00$ ls
101-compile  main.py  main.pyc
frank@ubuntu:~/py/0x00$ cat main.pyc | zgrep -c &quot;Best School&quot;
1
frank@ubuntu:~/py/0x00$ od -t x1 main.pyc # SYSTEM DEPENDANT =&gt; CAN BE DIFFERENT
0000000 ee 0c 0d 0a 91 26 3e 58 31 00 00 00 e3 00 00 00
0000020 00 00 00 00 00 00 00 00 00 02 00 00 00 40 00 00
0000040 00 73 0e 00 00 00 65 00 00 64 00 00 83 01 00 01
0000060 64 01 00 53 29 02 7a 10 48 6f 6c 62 65 72 74 6f
0000100 6e 20 53 63 68 6f 6f 6c 4e 29 01 da 05 70 72 69
0000120 6e 74 a9 00 72 02 00 00 00 72 02 00 00 00 fa 07
0000140 6d 61 69 6e 2e 70 79 da 08 3c 6d 6f 64 75 6c 65
0000160 3e 02 00 00 00 73 00 00 00 00
0000172
frank@ubuntu:~/py/0x00$ 
</code></pre>

<h3>13. ByteCode -&gt; Python #1</h3>
<p>Write the Python function <code>def magic_calculation(a, b):</code> that does exactly the same as the following Python bytecode:</p>

<pre><code>  3           0 LOAD_CONST               1 (98)
              3 LOAD_FAST                0 (a)
              6 LOAD_FAST                1 (b)
              9 BINARY_POWER
             10 BINARY_ADD
             11 RETURN_VALUE
</code></pre>

<ul>
<li>Tip: <a href="https://docs.python.org/3.4/library/dis.html" title="Python bytecode" target="_blank">Python bytecode</a></li>
</ul>

  </div>
