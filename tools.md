---
layout: default
---

# Tools and the IDE

---

## CS50 IDE
* [here](https://cs50.io/) it is
* [Is the Harvard IDE free for everyone?](https://www.quora.com/Is-the-Harvard-CS50-IDE-free-for-everyone) - yes!
* [lecture notes](https://cs50.harvard.edu/2018/fall/weeks/3/notes/#cs50-ide)
* [CS50 docs](https://cs50.readthedocs.io/ide/online/)
    * using the CS50 IDE [offline](https://cs50.readthedocs.io/ide/offline/)

---

## CS50's Tools
* [lecture notes](https://cs50.harvard.edu/2018/fall/weeks/3/notes/#tools)
* help50
    * a command-line program that translates many compiler and runtime error messages
        * for instance, you could use this tool to help you understand why hello.c wasn't compiling by running '''help50 make hello''' in your terminal (within the CS50 IDE)
        * you could run this command '''help50 ./hello''' for help with runtime error messages (like segmentation faults) with hello.c
    * an online version of this tool is available at [Help.CS50.net](https://help.cs50.net)
    * if interested, check out its [GitHub repo](https://github.com/cs50/help50) to see how it works underneath the hood!
* debug50
    * by setting breakpoints and walking through your program (and stepping into functions and such), you can use this tool to find bugs in your code!
* check50
    * tests the correctness (as per the problem specifications) of code
    * it also produces a suggestive automated correctness grade
        * so it's a good idea to run check50 before submitting your work!
    * [underneath the hood](check50(https://github.com/cs50/check50)
    * the checks themselves are open source; you can look through the ones for Fall 2018 [here](https://github.com/cs50/checks/tree/master/cs50/2018/fall)
        * it can be helpful to know how we are testing your program; it's also very important to run your own tests!
        * we usually check if your program exists (by looking in the folder you're in for a file with a specific name) and compiles before running a series of standard input/output checks (which are exactly what they sound like--we give your program some input and see if its output/behavior matches the staff solutions' output/behavior given the same input)
* style50
    * read about it [here](https://cs50.readthedocs.io/style50/#style50)
        * in particular, understand how to [use](https://cs50.readthedocs.io/style50/#usage) it and its [modes](https://cs50.readthedocs.io/style50/#modes)
    * [underneath the hood](https://github.com/cs50/style50)
    * it's based on CS50's [Style Guide](https://cs50.readthedocs.io/style/c/)
    * like check50, style50 produces a suggestive automated style grade
        * so it's also always a good idea to run style50 before submitting your work!
* submit50
    * what you'll use to submit (duh) your work
        * usage instructions are always detailed in a problem's specification
    * no need to understand how this works (you can just think of it as a wrapper for GitHub)
        * but if super curious, here it is [underneath the hood](https://github.com/cs50/submit50)
* compare50
    * also no need to understand how compare50 works; just know that we have a very sophisticated, "fast and extensible plagiarism detection tool"
        * [underneath the hood](https://github.com/cs50/compare50)
    * when people are very stressed or tired, they can make academically-dishonest mistakes; if you find yourself in this situation, do reach out to heads! :)
        * for more info, check out the [academic honesty](https://cs50.harvard.edu/2018/fall/syllabus/#academic-honesty) section in the syllabus
