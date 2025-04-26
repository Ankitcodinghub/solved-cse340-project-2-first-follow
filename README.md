# solved-cse340-project-2-first-follow
**TO GET THIS SOLUTION VISIT:** [SOLVED:CSE340 Project 2: FIRST & FOLLOW](https://www.ankitcodinghub.com/product/solvedproject-2-first-follow/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;1305&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SOLVED:CSE340  Project 2: FIRST \u0026amp; FOLLOW&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (1 vote)    </div>
    </div>
Abstract

Given a context-free grammar G as input, you are asked to write a program that calculatesFIRST and FOLLOW sets for all non-terminals of the grammar and determine if each of thenon-terminals in G generate a string of length 1.1 IntroductionIn this assignment, you will write a program that reads a context-free grammar from the standardinput and based on the command line argument passed to the program, compute one of the following:1. For all non-terminals of the input grammar, determine if the non-terminal can generate astring of length 1. For example, in the following grammar:S ! A S | S BA ! a | A aB ! A | b bwhere capital letters S, A, B are non-terminals and small letters a, b are terminals, S doesnot generate any string, A can generate a string of length 1 (A ) a) and B can generate astring of length 1 (B ) A ) a).2. Compute FIRST sets for all non-terminals of the input grammar.3. Compute FOLLOW sets for all non-terminals of the input grammar.

For FOLLOW sets you canassume that the grammar does not contain rules of the form A ! .Your program should read the input grammar from standard input (stdin), the input grammarformat is described in section 3. Additionally, a task number is passed to your program as acommand line argument. It specifies what to do with the input grammar. You need to read thevalue of the argument in your main() function and decide what to do with the input grammar.The tasks are numbered as follows:

1) Determine for each non-terminal of the grammar if it generates a string of length 1

2) Compute FIRST sets for all non-terminals of the grammar

3) Compute FOLLOW sets for all non-terminals of the grammar12 Reading Command-line ArgumentsThe following piece of code in C shows how to read the first command line argument and call afunction based on the argument value:

#include &lt;stdio.h#include &lt;stdlib.hint main (int argc, char* argv[]){int task;if (argc &lt; 2) {printf(“Error: missing argument\n”);return 1;}/* Note that argv[0] is the name of your executable* e.g. a.out, and the first argument to your program* is stored in argv[1]*/task = atoi(argv[1]);switch (task) {case

1:// Call the function(s) responsible for task 1 herebreak;case

2:// Call the function(s) responsible for task 2 herebreak;case

3:// Call the function(s) responsible for task 3 herebreak;default:printf(“Error: unrecognized task number %d\n”, task);break;}return 0;}3 Grammar DescriptionThe grammar specification has multiple sections separated by the # symbol. The grammar specificationis terminated with ##. If there are any symbols after the ##, they are ignored.

All grammar symbols as well as the # and ## symbols are whitespace-separated. The grammar description isdefined as follows:2grammar_description ! non_terminal_list rule_list DOUBLEHASHnon_terminal_list ! id_list HASHid_list ! ID id_listid_list ! IDrule_list ! rule rule_listrule_list ! rulerule ! ID ARROW righthand_side HASHrighthand_side ! id_listrighthand_side !

The tokens used in the grammar description are:ID = letter (letter + digit)*HASH = #DOUBLEHASH = ##ARROW = -Wheredigit = 0 + 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9letter = a + b + … + z + A + B + … + ZIn this project, we assume that there is at least one whitespace character (space, tab or newline)between any two tokens. This can make reading the input easier.

Also, tokens are case-sensitive.First Section: The first section of the input lists all the non-terminals of the grammar. The firstnon-terminal in this list is the start symbol of the grammar. Subsequent sections of the input eachrepresent a grammar rule.Grammar Rules:

A grammar rule starts with a non-terminal symbol (left-hand side of the rule)followed by -, then followed by a sequence of zero or more terminals and non-terminals whichrepresent the right-hand side of the rule. If the sequence of terminals and non-terminals in theright-hand side of a rule is empty, this represents a rule of the form A ! .3Here is an example input grammar:decl idList1 idList #decl – idList COLON ID #idList – ID idList1 #idList1 – #idList1 – COMMA ID idList1 # ##

The first section is the non-terminals list:NonTerminals = { decl, idList1, idList }And the rest of the input (terminated by the double-hash) specifies the grammar rules:decl ! idList COLON IDidList ! ID idList1idList1 ! iLlist1 ! COMMA ID idList1The list of terminals of the grammar consist of all ID tokens that appear in the grammar rulesand that are not non-terminals. In the example:Terminals = { COLON, ID, COMMA }Note: Even though the example shows that each rule is on a line by itself, a rule can be split intomultiple lines, or even multiple rules can be on the same line.

The formal specification given beforethe example defines the format of the input.4 String Generation TestGiven a non-terminal A, we say that A can generate a string of length one, if A =) a, where a isany terminal symbol of the grammar.Non-terminal A can generate a string of length 1 if any of the following holds:• A ! a where a is a terminal• A ! B where B is a non-terminal and B can generate a string of length one• A ! A1 A2 … An and there exists an i such that Ai is either a terminal or it can generatea string of length one and all other symbols in the right-hand-side can generate i.e. 8j 2{1, 2, …, n} \ {i}, Aj =)

Non-terminal A can generate

if any of the following holds:• A !

• A ! A1 A2 … An and all the right-hand-side symbols can generate

4To figure out which non-terminals in the grammar can generate a string of length 1, we need tostart by figuring out which non-terminals can generate

. One way to determine if a non-terminalgenerates

is to calculate the FIRST sets: A =)

if and only if 2 FIRST(A).

Here is an alternativemethod that does not depend on calculating FIRST sets:01 int num_symbols;02 int num_non_terminals;03 int num_terminals;04 int num_rules;0506 char *symbols[MAX_SYMBOLS];07 // in C++ you should use string vectors to store the symbols.08 // Using MAX_SYMBOLS is convenient but can lead to programming09 // errors and is not efficient memory-wise.

In the code below,10 // I assume that the symbols array has as first element a11 // representation of epsilon followed by a representation of EOF,12 // followed by all non-terminals and finally followed by all13 // terminals sorted according to dictionary order.1415 struct rule {16 int rhs_length;17 int LHS; // is the index of the non-terminal LHS in the symbols array18 int RHS[MAX_RHS_SIZE]; // RHS is an array of indices of RHS symbols19 }2021 gen_epsilon[0] = true; // the first symbol is epsilon and it has index 022 for (i = 1; i &lt; num_symbols; i++)23 gen_epsilon[i] = false;2425 // Find out which non-terminals can generate epsilon26 changed = true;27 while (changed)28 {29 changed = false; // if we change something, we will set changed to true30 for (i = 0; i &lt; num_rules; i++)31 {32 if ( gen_epsilon[rule[i].LHS] )33 continue;34 else if ( rule[i].rhs_length == 0 ) // A – epsilon35 {36 gen_epsilon[rule[i].LHS] = true;37 changed = true;38 }39 else // A – A1 A2 … An40 {41 some_does_not_gen_epsilon = false;42 for (j = 0; j &lt; rule[i].rhs_length; j++)43 some_does_not_gen_epsilon |= !gen_epsilon[rule[i].RHS[j]);4445 if (!some_does_not_gen_epsilon)46 {47 gen_epsilon[rule[i].LHS] = true;48 changed = true;49 }50 }51 }52 }5A similar approach can be used to determine which non-terminals generate strings of length 1.It is important in your work to have a representation of the symbols and the rules that can supportall parts of the project. The representation I have here is one possible representation if you areprogramming in C.5 RequirementsYour program should read the input grammar from standard input and print the requested outputto standard output. You should not open any files for reading or writing in your code. The testcase files are fed to your program with standard I/O redirection as explained in the documentcse340_S15_programming_projects.pdf.For each task (specified with the command line argument passed to your program) you needto output the result of your computations in a very specific manner described in this section.Your program should only generate the requested information (no debugging messages, no extrainformation) in the exact format specified here.5.1 Task 1: String Generation TestFor each of the non-terminals of the input grammar, in the order they appear in the non-terminalssection of the input, determine if the non-terminal generates a string of length 1 consisting solelyof terminals and output one line in the following format:&lt;symbol: &lt;resultWhere &lt;symbol should be replaced by the non-terminal and &lt;result should be either YES or NO.For example, for our sample grammar in section 3, we will have the following output:decl: NOidList1: NOidList: YES5.2 Task 2: FIRST SetsFor each of the non-terminals of the input grammar, in the order they appear in the non-terminalssection of the input, compute FIRST set for that non-terminal and output one line in the followingformat:FIRST(&lt;symbol) = { &lt;set_items }Where &lt;symbol should be replaced by the non-terminal and &lt;set_items should be replaced bythe comma-separated list of elements of the FIRST set ordered in the following manner:• If (represented by # in your output) belongs to the set, it should be listed before any otherelements• All other elements of the set should be sorted in dictionary orderFor our sample grammar from section 3, the output would be:6FIRST(decl) = { ID }FIRST(idList1) = { #, COMMA }FIRST(idList) = { ID }5.3 Task 3: FOLLOW SetsFor each of the non-terminals of the input grammar, in the order they appear in the non-terminalssection of the input, compute FOLLOW set for that non-terminal and output one line in the followingformat:FOLLOW(&lt;symbol) = { &lt;set_items }Where &lt;symbol should be replaced by the non-terminal and &lt;set_items should be replaced bythe comma-separated list of elements of the FOLLOW set ordered in the following manner:• If eof (represented by $ in your output) belongs to the set, it should be listed before anyother elements• All other elements of the set should be sorted in dictionary orderFor our sample grammar from section 3, the output would be:FOLLOW(decl) = { $ }FOLLOW(idList1) = { COLON }FOLLOW(idList) = { COLON }6 ImplementationIt is very important that you plan your implementation before you start coding. Read the specificationsa couple of times to make sure you understand what is required, then come up with adesign for your solution. At a high-level, your program will do the following:1. Read in the set of non-terminals and store them preserving their order.2. Read grammar rules and store them in appropriate data structures. While reading grammarrules, store new symbols (those that are not found in non-terminals) as terminals in thesymbol table.3. Read the command line argument to determine which computation is requested4. Based on the command line argument, do one of the following:• Determine for each of the non-terminals if they can generate a string of length 1 andoutput the results as specified in section 5.1.• Calculate FIRST sets for all non-terminals of the grammar and output the sets as specifiedin section 5.2.• Calculate FIRST sets for all non-terminals of the grammar, then calculate FOLLOW setsfor all non-terminals of the grammar. Then output only the FOLLOW sets as specified insection 5.3. You need to compute FIRST sets because they are needed for calculating theFOLLOW sets.7To calculate FIRST and FOLLOW sets you need to do a lot of set operations like intersectionand union. So you need a data structure to store sets and some functions to operate on set datastructures. A simple and efficient way of implementing a set data structure is to use fixed-lengthbinary arrays. For example, let’s say we want to represent the FIRST set of some symbol for theexample grammar given in section 3. A FIRST set can contain any one of the terminals of thegrammar and/or . So we consider a reference set that includes all terminals plus :U = { , COLON, COMMA, ID}Now if we want to store FIRST(idList), we can use the following binary array of length 4:FIRST(idList) = {0, 0, 0, 1}This binary array specifies which elements of the reference set are present in a subset of that referenceset. In this example, the only element present in FIRST(idList) is ID. This data structure is veryeasy to use and convenient for implementing set operations. For example if you want to implementset union operation, you can simply calculate the logical OR of the elements of the operands andif you want the intersection of two sets, you can simply use AND. Here is an example:A = {0, 1, 0, 1}B = {0, 0, 1, 1}A [ B = {0, 1, 1, 1}Be careful when using this technique, the operands should be subsets of the same reference set,otherwise the result is not meaningful. You will need a reference set for this project that containsall terminals plus and eof symbols (to represent both FIRST and FOLLOW sets). Note that theorder of elements in the reference set is important and should not change during the execution. Toconform to the order requirements given in section 5.2 and 5.3, you can first add # and $ to yourreference set and then add all terminals in alphabetic order.To run your program with a command line argument and redirect standard input to a test file usethe following command:$ ./a.out 1 &lt; test01.txtThis assumes that your executable is named a.out and you want to perform task 1 and the testfile test01.txt is located in the current working directory. Adjust the values to your needs.87 Grading1. Correctly doing the string generation test: 30 points2. Correctly calculating FIRST sets:(a) FIRST sets for grammars without : 25 points(b) FIRST sets for grammars with : 20 points3. Correctly calculating FOLLOW sets:(a) FOLLOW sets for grammars without : 25 points(b) (Bonus) FOLLOW sets for grammars with : 10 pointsThe distribution of points is not necessarily proportional to the difficulty.Your program will be executed 3 times for each test case with command line arguments 1, 2 and 3.In each execution, it should generate the appropriate output based on the command line argument.The generated output will be compared to the expected output for each task and it should matchthat expected output exactly, in order to get credit for the test case. A modified version of thetest script test1_p2.sh is provided on Blackboard and it can be used to test your code. If youhave not used the test script in Project 1, you should read about test scripts in the documentcse340_S15_programming_projects.pdf.To pass a test case, the output of the program should match the expected output. It is notenough that the right information be in the output that your program generates. The format andorder are essential.If you are unsure about the requirements, it is your responsibility to ask for clarification.8 Submission1. Only C or C++ can be used for this project2. You should submit all your code on the course website by 11:59:59 pm on due date.3. Make sure your submission has no compile problems. If after submission you get a compilererror on the website, fix the problem and submit again. A submission that does not compilewill not be given any credit4. You can submit any number of times you need, but remember that we only grade your lastsubmission5. Don’t include test scripts or test cases with your submission6. Don’t use any whitespace characters in your file names990
