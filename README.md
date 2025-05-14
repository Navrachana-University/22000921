Project title: The Garhwali compiler 

This is a basic compiler made using LEX and YACC for a custom language based on Garhwali words. The language uses simple keywords like kya_haal to start the program, feri_malya to end it, bol to declare variables, and bol_de to print messages. It also supports if-else conditions using agar, toh, and nahi_toh. The LEX file helps break the input into tokens, while the YACC file checks the structure of the program and generates intermediate code. The output shows step-by-step instructions similar to how a real compiler works.

Steps to run the project code:

1.Download the following files and save in one folder (garhwali.l, garhwali.y, program.grw)

2.Open command prompt and type cd path\to\your\folder

3.Then run the steps 4-7 and your three address code will be generated.

4.flex garhwali.l

5.bison -d garhwali.y

6.gcc lex.yy.c garhwali.tab.c -o garhwali_compiler

7.Get-Content program.grw | ./garhwali_compiler


