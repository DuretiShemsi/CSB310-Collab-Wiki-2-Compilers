# Compilers: An Overview

Rory Hackney  
Max Cifuentes  
Dureti Shemsi  



Compilers provide a way for a code to be written in a higher-level language, but then can be translated to be  understood by the computer in machine language. This allows for coding to progress faster because writing in machine  code can be very tedious when compared to using a higher-level language like Java. The first compiler arose from Grace   Hooper, whose A-O compiler in the 1950s would take math code and turn it into machine language that could be run by a   computer. Although it wasn’t used for any programing language, it set the basis for a programming language, FORTRAN.   IBM’s FORTRAN (1957) was the first complete compiler that allowed for code written that is more higher-level, more human   understandable language and then be converted into machine code that could be executed. This development meant that  future languages would follow suit, and also begin to develop their compilers for ease of use on the human coder’s  part   


The first compilers were almost exclusively self-hosted, with the first of those languages being Lisp (1962). A self-  hosted language is a language that is powerful enough to create its own compiler with its own syntax. This became famously known as the bootstrapping problem where you have to have a compiler for a higher-level language, while the  language must be capable of being able to create a compiler in the first place. Future languages would also follow in Lisp’s  footsteps by creating their own compilers using the language itself like in the case of Java or C++. Although these days, it is    sometimes changed up a bit where a more established language is used to create an initial compiler for a new, develop  language until a time that that new language can make its own compiler.   

Future compilers would also make use of optimization in their work, where the compiler analyzes the code provided  and optimizes it to get better performance. While it’s not perfect if the initial code put into it was poorly designed, it does   enhance the code by deciding what code doesn’t actually impact  the output, and making it disappear while also taking  things like a loop and optimizing them for the hardware. Most compilers in our modern era typically use a form of  optimization in one way or another when performing their work to make the process of compilation and execution quicker.   When taken with other tools like Just in Time (JIT) compilation, wherein code is dynamically compiled during execution,   optimization and JIT allow for much faster compilation times and allow for our code to begin executing with much less delay. 


# Bibliography

[1] P. Pawar, “History of compiler design,” Medium, Oct. 20, 2021, https://medium.com/@PowerPP/history-of-compiler-design-c48bfa78122e (accessed Apr. 27, 2024).

[2] GeeksforGeeks, “History of compiler,” GeeksforGeeks, Feb. 22, 2023 https://www.geeksforgeeks.org/history-of-compiler/ (accessed Apr. 27, 2024). 
