# Compilers: An Overview

Rory Hackney  
Max Cifuentes  
Dureti Shemsi  



Compilers provide a way for a code to be written in a higher-level language, but then can be translated to be  understood by the computer in machine language. This allows for coding to progress faster because writing in machine  code can be very tedious when compared to using a higher-level language like Java. The first compiler arose from Grace   Hooper, whose A-O compiler in the 1950s would take math code and turn it into machine language that could be run by a   computer. Although it wasn’t used for any programing language, it set the basis for a programming language, FORTRAN.   IBM’s FORTRAN (1957) was the first complete compiler that allowed for code written that is more higher-level, more human   understandable language and then be converted into machine code that could be executed. This development meant that  future languages would follow suit, and also begin to develop their compilers for ease of use on the human coder’s  part   


The first compilers were almost exclusively self-hosted, with the first of those languages being Lisp (1962). A self-  hosted language is a language that is powerful enough to create its own compiler with its own syntax. This became famously known as the bootstrapping problem where you have to have a compiler for a higher-level language, while the  language must be capable of being able to create a compiler in the first place. Future languages would also follow in Lisp’s  footsteps by creating their own compilers using the language itself like in the case of Java or C++. Although these days, it is    sometimes changed up a bit where a more established language is used to create an initial compiler for a new, develop  language until a time that that new language can make its own compiler.   

Future compilers would also make use of optimization in their work, where the compiler analyzes the code provided  and optimizes it to get better performance. While it’s not perfect if the initial code put into it was poorly designed, it does   enhance the code by deciding what code doesn’t actually impact  the output, and making it disappear while also taking  things like a loop and optimizing them for the hardware. Most compilers in our modern era typically use a form of  optimization in one way or another when performing their work to make the process of compilation and execution quicker.   When taken with other tools like Just in Time (JIT) compilation, wherein code is dynamically compiled during execution,   optimization and JIT allow for much faster compilation times and allow for our code to begin executing with much less delay. 

## Types of Compilers
Compilers can be divided into three types: single-pass, two-pass, and multi-pass. The number of passes refers to how many times
the compiler reads the file to be compiled. Generally, there is a trade-off between speed of compilation and optimization, where
fewer passes are able to process the file faster but more passes are better able to optimize the code, as well as some other benefits.

In single-pass compilers, also known as narrow compilers, the file is processed only once. This makes single-pass compilers the
most efficient. However, the compiled file is not optimized. The source code is simply converted into machine code, without attempting
to improve the performance of the generated file. Since this type of compiler only processes the file once, its understanding of
context of a line of code is limited, and these compilers are generally used for languages with simpler grammars. One example of a
language that uses a single-pass compiler is Pascal.

In two-pass compilers, the file is processed twice. The two phases are usually called front-end and back-end. During front-end,
which is the platform independent portion, the code is analyzed and turned into tokens, building the symbol table. During back-end,
tokens are replaced with values, and code is checked for syntax errors and turned into optimized, machine dependent machine code.

In multi-pass compilers, also known as wide compilers, the file is multiplied multiple times, allowing the compiler to fully optimize
the resulting compiled file. Each pass reads and writes an intermediate file which is used by the next pass. By splitting the compilation
up into multiple passes, the compiler is able to separate machine dependent steps from machine independent steps. This is how Java's
virtual machine is done, with the final compilation into machine dependent code being separate and specific to the machine.

## Compilation vs Interpretation
Although so far this has focused on compilers, there is an alternative known as interpreters. These fundamentally approach the task of
translating high level coding languages into machine code differently. While a compiler must translate the entire project into machine
code, interpreters instead translate and run one line at a time. This allows for faster development and testing, since it does not require
rebuilding the project after every change. However, interpreted code runs up to 10x slower than compiled code, though as previously mentioned,
Just In Time compilation is shrinking this divide.

When performance is important, compiled languages are a better choice as fully compiled files run much faster than interpreted files.
For example, scientific / big data processing like weather prediction, or in limited resource environments, like embedded systems,
compiled languages are best. However, intepreted languages have their strengths as well, and are often used in applications where
performance is not critical, like server side development and user interfaces (UI) because it's often easier to develop programs using
interpreted languages, like Python.

Commonly known interpreted languages include Python, PHP, and JavaScript, while some examples of compiled languages include Java, C++, and Rust.

# Bibliography

[1] P. Pawar, “History of compiler design,” Medium, Oct. 20, 2021, https://medium.com/@PowerPP/history-of-compiler-design-c48bfa78122e (accessed Apr. 27, 2024).

[2] GeeksforGeeks, “History of compiler,” GeeksforGeeks, Feb. 22, 2023 https://www.geeksforgeeks.org/history-of-compiler/ (accessed Apr. 27, 2024). 

[3] FreeCodeCamp. “Interpreted vs Compiled Programming Languages: What’s the Difference?” FreeCodeCamp.org, Free Code Camp, 10 Jan. 2020, www.freecodecamp.org/news/compiled-versus-interpreted-languages/. Accessed 29 Apr. 2024.

[4] Geeksforgeeks. “Single Pass, Two Pass, and Multi Pass Compilers.” GeeksforGeeks, Geeks For Geeks, 13 Mar. 2019, www.geeksforgeeks.org/single-pass-two-pass-and-multi-pass-compilers/. Accessed 29 Apr. 2024.

[5] Khatri, Vinay. “What Is a Compiler? Definition, Phases, and Various Types.” Techgeekbuzz.com, Tech Geek Buzz, 6 July 2019, www.techgeekbuzz.com/blog/what-is-compiler/. Accessed 29 Apr. 2024.

[6] Limón, Bryce. “Compiled vs Interpreted Language: Basics for Beginning Devs.” Educative: Interactive Courses for Software Developers, Educative, 26 July 2022, www.educative.io/blog/compiled-vs-interpreted-language. Accessed 29 Apr. 2024.

[7] Lithmee. “What Is the Difference between Single Pass and Multipass Compiler.” Pediaa.com, Pediaa, 20 Nov. 2018, pediaa.com/what-is-the-difference-between-single-pass-and-multipass-compiler/. Accessed 29 Apr. 2024.