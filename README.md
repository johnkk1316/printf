
# 0x11. C - printf

A Team Project for alx software engineering program
using C language to build a custom printf function


## Contributors
1. John Kinyanjui
https://github.com/johnkk1316

2. Peter Ani
Github: https://github.com/vortex-hue
## Acknowledgements

 - [Peer Programming](https://alx-intranet.hbtn.io/concepts/121)
 - [Secret of Printf](https://alx-intranet.hbtn.io/rltoken/7Vw7aUWgwC7JYUrqI4bh4Q)
 - [Google](https://google.com/)


## Authors

- [@John](https://github.com/johnkk1316)
- [@Peter](https://www.github.com/vortex-hue)


## Description
This is a group project by me and peter.
It's part of our requirements for passing c alx
software engineering program.

This is a peer project


# 0x11. C - printf

A Team Project for alx software engineering program
using C language to build a custom printf function


## Contributors
1. john Kinyanjui
https://github.com/johnkk1316

2. Peter Ani
Github: https://github.com/vortex-hue
## Acknowledgements

 - [Peer Programming](https://alx-intranet.hbtn.io/concepts/121)
 - [Secret of Printf](https://alx-intranet.hbtn.io/rltoken/7Vw7aUWgwC7JYUrqI4bh4Q)
 - [Google](https://google.com/)


## Authors

- [@John](https://github.com/johnkk1316)
- [@Peter](https://www.github.com/vortex-hue)


## Description
This is a group project by me and jason.
It's part of our requirements for passing c alx
software engineering program.

This is a peer project
## Pseudocode
<blockquote><p><span style="color: #000000;"><strong>Module&nbsp;1:&nbsp;Initializing a variadic function </strong></span></p></blockquote>
<p style="text-align: justify;"><span style="color: #000000;">In this section, we initialize the arguments of Myprintf( ) function by using standard argument library.</span></p>
<pre class="lang:default decode:true ">va_list arg;</pre>
<p style="text-align: justify;"><span style="color: #000000;">This line declares a variable, <strong>arg</strong>, which we use to&nbsp;manipulating the argument list containing variable arguments of Myprintf( ). The data type of the variable is va_list, a special type defined by &lt;stdarg.h&gt;.</span></p>
<pre class="lang:default decode:true">va_start(arg, format);
</pre>
<p style="text-align: justify;"><span style="color: #000000;">This line initializes <tt><strong>arg</strong> variable with&nbsp;</tt>function’s last fixed argument i.e. <strong>format</strong>. <tt>va_start()</tt> uses this to figure out where the variable arguments begin.</span></p>
<blockquote>
<p style="text-align: justify;"><span style="color: #000000;"><strong>Module&nbsp;2: Fetching and executing arguments</strong></span></p>
</blockquote>
<pre class="lang:default decode:true ">i = va_arg(arg,int);</pre>
<p style="text-align: justify;"><span style="color: #000000;">va_arg() fetches the next argument from the argument list. The second parameter&nbsp;to va_arg() is the <strong>data type</strong> of the argument we expect.&nbsp;</span></p>
<p style="text-align: justify;"><span style="color: #000000;">Note:&nbsp;va_arg( ) function will never receive arguments of type char, short int, or float. va_arg( ) function only accept arguments of type char *, unsigned int, int or double.</span></p>
<blockquote>
<p style="text-align: justify;"><span style="color: #000000;"><strong>Module 3: Closing argument list to necessary clean-up</strong></span></p>
</blockquote>
<pre class="">	va_end(arg);
</pre>
<p style="text-align: justify;"><span style="color: #000000;">Finally, when we’re finished processing the all arguments, we call <tt>va_end()</tt>, which performs any necessary cleanup.</span></p>

