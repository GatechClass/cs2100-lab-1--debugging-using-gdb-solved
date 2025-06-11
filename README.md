# cs2100-lab-1--debugging-using-gdb-solved
**TO GET THIS SOLUTION VISIT:** [CS2100 Lab #1- Debugging using GDB Solved](https://mantutor.com/product/cs2100-computer-organisation-solved-6/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112862&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2100 Lab #1- Debugging using GDB Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
___

SPECIAL NOTE FOR APPLE SILICON MACOS USERS

GDB does not work on MacOS on Apple Silicon (M1 or M2) MacBooks. If you are using an M1 or M2 based MacOS system, you have two choices:

https://www.parallels.com/landingpage/pd/education/

ii) Use LLDB instead. The commands aren’t exactly the same, but you should be able to accomplish the steps below using equivalent commands, though it will be harder work for you. You can find an LLDB tutorial here: https://lldb.llvm.org/use/tutorial.html

GNU Debugger (GDB) https://www.gnu.org/software/gdb/

A debugger is used to analyze program execution in a step-by-step and detailed manner. It is used to find bugs in a program. Using a debugger, we can execute a program partially and view the status of the variables and resources being used the program to identify any discrepancies. GDB is an open source, freely available debugger which can be used for multiple languages.

GDB can do four main kinds of things (plus other things in support of these) to help you catch bugs in the act:

• Start your program, specifying anything that might affect its behaviour.

• Make your program stop on specified conditions.

• Examine what has happened, when your program has stopped.

• Change things in your program; so that you can experiment with correcting the effects of one bug and go on to learn about another.

GNU Compiler Collection (GCC)

GCC is an open-source compiler system used to compile C/C++ programs: https://gcc.gnu.org/ Objective: You will learn how to use GDB to debug a C program.

Preparation (before the lab):

1. Install GDB:

a. Ubuntu: sudo apt-get install gdb

b. OSX: brew install gdb (Does not work on Apple Silicon. See special note above.) c. Windows:

• Download Cygwin (https://cygwin.com/install.html)

Note: The installer will ask you to choose a mirror to download from. If possible, choose https://download.nus.edu.sg. If this is not available, choose an Australian or US server as these are generally faster.

• Select develop packages during installation:

• Start Cygwin terminal from the start menu:

2. Starting GDB (all platforms): Type GDB in the terminal (Cygwin terminal for windows users). Help command lists the help and quit command exits GDB.

Procedure:

1. Download the file lab1.c from Canvas.

2. Compile lab1.c with gcc using the following command: gcc –g –o lab1 lab1.c

3. What is the purpose of the flags “g” and “o” in gcc?

4. Execute the program you just compiled using the command: ./lab1 (for windows type: lab1). What is the error encountered (if any!)?

Answer: ______________________________________________________

5. Start the GDB debugger by using the command: gdb lab1

6. To run the program in GDB, you can use the command run. This will run the whole program without any pause. Type run to execute the program.

7. To get into the debug mode use the start command

• You can use the list command to view the source code at any point

• You can also use layout src and layout asm commands to view source code and assembly code in a split screen.

8. A breakpoint is a command to put an intentional pause in the program execution to inspect the variable values and resources in the program. You can set multiple breakpoints in a program. In GDB you can put a breakpoint at any line number using the command:

&gt; break lineNumber or &gt; b lineNumber

Example: This will put a breakpoint on line 6 &gt; break 6

Now if you run the program, it will pause at line 6. You can continue execution (till end or the next breakpoint) using the continue command.

Which line(s) will you set the breakpoint(s) in?

Answer: ___________________________________________________________

9. A step command is used to carry out step-by-step execution of the program. You can step through the program using the following command:

&gt; step

This will execute only the next line of code or

&gt; step numberOfLines

E.g. &gt; step 3 will execute next three lines of code

• You can “switch on” display of the associated assembly code related to the instruction being executed using the command: set disassemble-next-line on

10. At every step (or breakpoint) you can view a variable value using the print command:

&gt; print a

You can view all local variable values using the command:

&gt; info locals

What are the values of variables c and d at the start of line 8 (before executing line 8)?

Answers: _______________________________________________________________

11. You can view the register values at any step or breakpoint using this command:

&gt; info registers

12. You can stop the debugging by using the stop command. To quit GDB, use the quit command.

13. Debug and modify lab1.c to carry out four arithmetic operations (+, -, /, *) and print the days of the week. The output of the program should look as follows:

The code lab1.c is also shown on the next page for your reference.

Show your labTA the output of your corrected program.

14. Submit this report to your labTA at the end of the lab. You do not need to submit the corrected program. You are not to email the report to your labTA.

Program lab1.c

#include &lt;stdio.h&gt;

int main(void){

int a = 10; int b = 10; int c = a+b; int d = a-b; int e = a/d; int f = a*b; int i;

char *day[7] = {

};

printf(“Arithmetic operations: “); printf(“a+b = %d “, c); printf(“a-b = %d “, d); printf(“b/a = %d “, e); printf(“a*b = %d “, f);

printf(“Days of the week: “); for (i=0; i&lt;8; i++) {

printf(“Day[%d] = %s “, i, day[i]);

}

return 0;

}
