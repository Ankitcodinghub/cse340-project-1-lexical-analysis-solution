# cse340-project-1-lexical-analysis-solution
**TO GET THIS SOLUTION VISIT:** [CSE340 Project 1: Lexical Analysis Solution](https://www.ankitcodinghub.com/product/cse340-project-1-lexical-analysis-solution/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;9136&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE340 Project 1: Lexical Analysis Solution&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<h1>Introduction</h1>
The goal of this project is to show you how a description of a list of tokens can be used to automatically generate a lexical analyzer. The input to your program will be a description of tokens using regular expressions together with a text. Your program will generate data structures that will allow it to do lexical analysis on the text according to the tokens. The output of the program will be a list of tokens or an error message if the input does not have the correct format.

<h1>Input Format</h1>
The input of your program is specified by the following context-free grammar:

<table width="650">
<tbody>
<tr>
<td width="144">input</td>
<td width="64"><em>→</em></td>
<td width="442">tokens_sectionINPUT_TEXT</td>
</tr>
<tr>
<td width="144">tokens_section</td>
<td width="64"><em>→</em></td>
<td width="442">token_listHASH</td>
</tr>
<tr>
<td width="144">token_list</td>
<td width="64"><em>→</em></td>
<td width="442">token</td>
</tr>
<tr>
<td width="144">token_list</td>
<td width="64"><em>→</em></td>
<td width="442">token COMMA token_list</td>
</tr>
<tr>
<td width="144">token</td>
<td width="64"><em>→</em></td>
<td width="442">ID expr</td>
</tr>
<tr>
<td width="144">expr</td>
<td width="64"><em>→</em></td>
<td width="442">CHAR</td>
</tr>
<tr>
<td width="144">expr</td>
<td width="64"><em>→</em></td>
<td width="442">LPAREN expr RPAREN DOT LPAREN expr RPAREN</td>
</tr>
<tr>
<td width="144">expr</td>
<td width="64"><em>→</em></td>
<td width="442">LPAREN expr RPAREN OR LPAREN expr RPAREN</td>
</tr>
<tr>
<td width="144">expr</td>
<td width="64"><em>→</em></td>
<td width="442">LPAREN expr RPAREN STAR</td>
</tr>
<tr>
<td width="144">expr</td>
<td width="64"><em>→</em></td>
<td width="442">UNDERSCORE</td>
</tr>
</tbody>
</table>
Where

<table width="650">
<tbody>
<tr>
<td width="650">CHAR&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; =&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; a | b | … | z | A | B | … | Z | 0 | 1 | … | 9

LETTER&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; =&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; a | b | … | z | A | B | … | Z

SPACE&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; = ‘ ‘ | \n | \t

INPUT_TEXT = ” . (CHAR | SPACE)* . ”

COMMA = ‘,’ LPAREN = ‘(‘ RPAREN = ‘)’ STAR = ‘*’

DOT&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; = ‘.’ OR&nbsp;&nbsp; = ‘|’ UNDERSCORE = ‘_’

ID&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; = LETTER . CHAR*
</td>
</tr>
</tbody>
</table>
In the description of regular expressions, UNDERSCORE represents epsilon.

<h2>Examples</h2>
The following are examples of input.

<ol>
<li>t1 (a)|(b) , t2 (a)* , t3 (((a)|(b))*).((c)*) #</li>
</ol>
“a aa bb aab”

This input specifies three tokens t1, t2, and t3 and an INPUT_TEXT “a aa bb aab”.

<ol start="2">
<li>t1 (a)|(b) , t2 (a)* #</li>
</ol>
“a aa bb aad aa”

This input specifies two tokens t1, t2, and an INPUT_TEXT “a aa bb aad aa”.

<ol start="3">
<li>t1 (a)|(b) , t2 (a)* , t3 (((a)|(b))*).(((c)|(d))*)#</li>
</ol>
“aaabbcaaaa”

This input specifies three tokens whose names are t1, t2, and t3 and an INPUT_TEXT “aaabbcaaaa”.

<h2>Note</h2>
The input format can be confusing because there are two kinds of tokens.

<ol>
<li>There are tokens that are used in describing the input format such as ID and CHAR. When your program read them input, it will repeatedly call lexer.getToken() to get the sequence of tokens in the input and parse the various sections of the input according to the provided grammar.</li>
<li>The input itself has a description of tokens by providing the names of these tokens and the regular expressions of each token. These tokens whose description is provided in the input will be used to breakdown INPUT_TEXT (the last section of the input) as a sequence of tokens according to the token_list in the input description.</li>
</ol>
You should not confuse the two kinds of tokens.

<h1>Output Format</h1>
The output will be a sequence of tokens and their corresponding lexemes according to the list of tokens provided in the input or SYNTAX ERROR:

<ol>
<li>if the input to your program is in the correct format, the program should do lexical analysis on INPUT_TEXT and should produce a sequence of tokens and lexemes in INPUT_TEXT according to the list of tokens specified in the input to your program. Each token and lexeme should be printed on a separate line. The output on a given line will be of the form t , “lexeme”</li>
</ol>
where t is the name of a token and lexeme is the actual lexeme for the token t. If during lexical analysis of INPUT_TEXT, a syntax error is encountered then ERROR is printed on a separate line and the program exits.

In doing lexical analysis for INPUT_TEXT, SPACE is treated as a separator and is otherwise ignored.

<ol start="2">
<li>if the input to your program is not in the correct format, the program should output SYNTAX ERROR and nothing else</li>
</ol>
<h2>Examples</h2>
Each of the following examples gives an input and the corresponding expected output.

<ol>
<li>t1 (a)|(b) , t2 (a)* , t3 (((a)|(b))*).((c)*) #</li>
</ol>
“a aa bb aab”

This input specifies three tokens t1, t2, and t3 and an INPUT_TEXT “a aa bb aab”. Since the input is in the correct format, the output of your program should be the list tokens in the INPUT_TEXT: t1 , “a” t2 , “aa” t3 , “bb” t3 , “aab”

<ol start="2">
<li>t1 (a)|(b) , t2 (a)* , t3 (((a)|(b))*).((c)*) #</li>
</ol>
“a aa bb aad aa”

Since the input is in the correct format, the output of your program should be the list tokens in the INPUT_TEXT the output of the program should be

t1 , “a” t2 , “aa” t3 , “bb” t2 , “aa”

ERROR

Note that the input is in the correct format, but doing lexical analysis for INPUT_TEXT according to the list of tokens produces ERROR after the second t2 token because there is no token that starts with ’d’.

<ol start="3">
<li>t1a (a)|(b) , t2bc (a)* , t34 (((a)|(b))*).(((c)|(d))*)# “aaabbcaaaa”</li>
</ol>
This input specifies three tokens whose names are t1a, t2bc, and t34 and an input text “aaabbcaaaa”. Since the input is in the correct format, the output of your program should be the list tokens in the INPUT_TEXT:

t34 , “aaabbc” t2bc , “aaaa”

<h1>Requirements</h1>
You should write a program to generate the correct output for a given input as described above.

You will be provided with a number of test cases. Since this is the first project, the number of test cases provided with the project will be relatively large.

<strong>In your solution, you are not allowed to use any built-in or library support for regular expressions in C/C++. This requirement will be enforced by checking your code.</strong>

<h1>How to Implement a Solution</h1>
The main difficulty in coming up with a solution is to transform a given list of token names and their regular expression descriptions into a getToken() function for the given list of tokens. This transformation will be done in three high-level steps:

<ol>
<li>Transform a regular expression into an NFA. The goal here is to parse a regular expression description and generate a graph that represents the regular expression<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>. The generated graph will have a specific format and I will describe below how to generate it. In what follows I will call it a <em><sub>regular expression</sub></em></li>
</ol>
<em>graph</em>, or REG for short.

Figure 1: Regular expressions graphs for the base cases

Figure 2: Regular expression graph for the an expression obtained using the dot operator

<ol start="2">
<li>Write a function match(r,s,p), where r is a REG , s is a string and p is a position in the string s. The function match will return the longest possible lexeme starting from position p in the string s that matches the regular expression of the graph r.</li>
<li>Write a class LexicalAnalyzer(list,s) where list is a list of structures: <em>{</em>token_name<em>,reg</em>_<em><sub>pointer</sub>} </em>and s is an input string. LexicalAnalyzer stores the list of structures and keeps track of the part of the input string that has been processed. Lexical analyzer has a method getToken(). For every call of getToken(), match(r,s,p) is called for every REG <em><sub>r </sub></em>in the list starting from the current position p maintained in the lexical analyzer. getToken() returns the token with the longest matching prefix together with its lexeme longest and updates the current position. If the longest matching prefix matches more than one token, the matched token that is listed first in the list of tokens is returned. In what follows I describe how a regular expression description can be transformed into a REG and how to implement the function match(r,s,p).</li>
</ol>
<h2>Constructing REGs</h2>
The construction of REGs is done recursively. The construction we use is called Thompson’s construction. Each REG has a one starting node and one final node. For the base cases of epsilon and a, the REGs are shown in Figure 1. For the recursive cases, the constructions are shown in Figures 2, 3, and 4. An example REG for the regular expression ((a)*).((b)*) is shown in Figure 5.

<h3>Data Structures and Code for REGs</h3>
In the construction of REGs, every node has at most two outgoing arrows. This will allow us to use a simple representation of a REG node.

Figure 3: Regular expression graph for the an expression obtained using the or operator

Figure 4: Regular expression graph for the an expression obtained using the star operator

struct REG_node { struct REG_node * first-neighbor; char first_label;

struct REG_node * second_neighbor; char second_label; }

In the representation, first_neighbor is the first node pointed to by a node and second_neighbor is the second node pointed to by a node. first_label and second_label are the labels of the arrows from the node to its neighbors. If a node has only one neighbor, then second_neighbor will be NULL. If a node has no neighbors, the both first_neighbor and second_neighbor will be NULL.

struct REG { struct REG_node * starting;

struct REG_node * accepting;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // note that I changed final to accepting because final // is reserved in C++ }

Figure 5: Regular expression graph for the an expression obtained using concatenation and star operators

The function parse_regular_expr() should not only parse a regular expression, but should also return the REG of the regular expression that is parsed. The construction of REGs is done recursively. An outline of the process is shown on the next page.

struct REG * parse_regular_expression()

{

// if expression is UNDERSCORE or a CHAR, say ‘a’ for example

// create a REG for the expression and return it

// (see Figure 1, for how the REG looks like)

// if expression is (R1).(R2)

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the program will call parse_regular_expr() twice, once

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to parse R1 and once to parse R2

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Each of the two calls will return a REG, say they are

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; r1 and r2

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; construct a new REG r for (R1).(R2) using the

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; two REGs r1 and r2

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (see Figure 2 for how the two REGs are combined)

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return r

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the cases for (R1)|(R2) and (R)* are similar

}

<h3>Detailed Examples for REG Construction</h3>
I consider the regular expression ((a)*).((b)*) and explain step by step how its REG is constructed (Figure 5).

When parsing the ((a)*).((b)*), the first expression to be parsed is a and its REG is constructed according to Figure 1. In Figure 5, the nodes for the REG of the regular expression a have numbers 1 and 2 to indicate that they are the first two nodes to be created.

The second expression to be parsed when parsing ((a)*).((b)*) is (a)*. The REG for (a)* is obtained from the REG for the regular expression a by adding two more nodes (3 and 4) and adding the appropriate arrows as described in the general case in Figure 4. The starting node for the REG of (a)* is the newly created node 3 and the accepting node is the newly created node 4.

The third regular expression to be parsed while parsing ((a)*).((b)*) is the regular expression b. The REG for regular expression b is constructed as shown in Figure 1. The nodes for this REG are numbered 5 and 6. The fourth regular expression to be parsed while parsing ((a)*).((b)*) is (b)*. The REG for (b)* is obtained from the REG for the regular expression b by adding two more nodes (7 and 8) and adding the appropriate arrows as described in the general case in Figure 4. The starting node for the REG of (b)* is the newly created node 7 and the accepting node is the newly created node 8.

Finally, the last regular expression to be parsed is the regular expression ((a)*).((b)*). The REG of ((a)*).((b)*) is obtained from the REGs of (a)* and (b)* by creating a new REG whose initial node is node 3 and whose accepting node is node 8 and adding an arrow from node 4 (the accepting node of the REG of (a)*) to node 7 (the initial node for the REG of (b)*).

Another example for the REG of (((a)*).((b).(b)))|((a)*) is shown in Figures 7 and 8. In the next section, I will use this example to illustrate how match(r,s,p) can be implemented.

<h2>Implementing match(r,s,p)</h2>
Given an REG r, a string s and a position p in the string s, we would like to determine the longest possible lexeme that matches the regular expression for r.

As you will see in CSE355, a string w is in L(R) for a regular expression R with REG r if and only if there is a path from the starting node of r to the accepting node of r such that w is equal to the concatenation of all labels of the edges along the path. I will not into the details of the equivalence in this document. I will describe how to find the longest possible substring w of s starting at position p such that there is a path from the starting node of r to the accepting node of r that can be labeled with w.

To implement match(r,s,p), we need to be able to determine for a given input character a and a set of nodes S the set of nodes that can be reached from nodes in S by <em><sub>consuming </sub></em>a. To consume a we can traverse any number of edges labeled ’_’, traverse one edge labeled a, then traverse any number of edges labeled ’_’.

At each step, the solution will keep track of the set of nodes S that can be reached by consuming a prefix of the input string so far. Initially S is the set of nodes that can be reached from the starting node by not consuming any input (empty prefix).

For a given character a and a given set S, the solution will find all the nodes that can be reached from S by consuming a. This will be implemented in a function that can be called match_one_char() shown in Figure 6.

To implement match(r,s,p), we start with the set of nodes that can be reached from the starting node of r by consuming no input. Then we repeatedly call match_one_char() for successive characters of the string s starting from position p until the returned set of nodes S is empty or we run out of input. If at any point during the repeated calls to match_one_char() the set S of nodes contains the accepting node, we note the fact that the prefix of string s starting from position p up to the current position is matching. At the end of the calls to match_one_char() when S is empty or the end of input is reached, the last matched prefix is the one returned by match(r,s,p). If none of the prefixes are matched, then there is no match for r in s starting at p.

set_of_nodes match_one_char(set_of_nodes S, char c)

{

// 1. find all nodes that can be reached from S by consuming c

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; S’ = empty set

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for every node n in S

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ( (there is an edge from n to m labeled with c) &amp;&amp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ( m is not in S) ) {

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; add m to S’

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (S’ is empty)

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return empty set

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; At this point, S’ is not empty and it contains the nodes that

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; can be reached from S by consuming the character c directly

//

//

// 2. find all all nodes that can be reached from the resulting

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; set S’ by consuming no input

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; changed = true

// while (changed) { // changed = false

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for every node n in S’

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ( (there is an edge from n to m labeled with ‘_’) &amp;&amp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ( m is not in S’) ) {

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; add m to S’

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; changed = true

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }

//

// at this point the set S’ contains all nodes that can be reached //&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; from S by first consuming C, then traversing 0 or more epsilon

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; edges

//

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return S’

}

Figure 6: Pseudocode for matching one character

.

<strong>Note</strong>. The algorithms given above are not the most efficient, but they are probably the simplest to implement the matching functions.

<h2>Detailed Example for Implementing match(r,s,p)</h2>
In this section, I illustrate the steps of an execution of match(r,s,p) on the REG of (((a)*).((b).(b)))|((a)*) shown in Figure 8. The input string we will consider is the string s = “aaba” and the initial position is p =

<ol>
<li>1. Initially</li>
</ol>
The set of states that can reached by consuming no input starting from node 17 is <em><sub>S</sub></em><sub>0 </sub>= <em><sub>{</sub></em>17<em><sub>,</sub></em>3<em><sub>,</sub></em>1<em><sub>,</sub></em>4<em><sub>,</sub></em>9<em><sub>,</sub></em>15<em><sub>,</sub></em>13<em><sub>,</sub></em>16<em><sub>,</sub></em><strong><sub>18</sub></strong><em><sub>} </sub></em>Note that <em><sub>S</sub></em><sub>0 </sub>contains node <strong><sub>18 </sub></strong>which means that the empty string is a matching prefix.

<ol start="2">
<li>Consuming a</li>
</ol>
The set of states that can be reached by consuming a starting from <em><sub>S</sub></em><sub>0 </sub>is <em><sub>S</sub></em><sub>1 </sub>= <em><sub>{</sub></em>2<em><sub>,</sub></em>14<em><sub>}</sub></em>

Figure 7: Regular expression graph ((a)*).((b).(b))

Figure 8: Regular expression graph (((a)*).((b).(b)))|((a)*)

The set of states that can be reached by consuming no input starting from <em><sub>S</sub></em><sub>1 </sub>is <em><sub>S</sub></em><sub>1_ </sub>= <em>{</em>2<em><sub>,</sub></em>1<em><sub>,</sub></em>4<em><sub>,</sub></em>9<em><sub>,</sub></em>14<em><sub>,</sub></em>13<em><sub>,</sub></em>16<em><sub>,</sub></em><strong><sub>18</sub></strong><em>} </em>Note that <em><sub>S</sub></em><sub>1_ </sub>contains node <strong><sub>18</sub></strong>, which means that the prefix “a” is a matching prefix. 3. Consuming a

The set of states that can be reached by consuming a starting from <em><sub>S</sub></em><sub>1_ </sub>is <em><sub>S</sub></em><sub>2 </sub>= <em>{</em>2<em><sub>,</sub></em>14<em>}</em>

The set of states that can be reached by consuming no input starting from <em><sub>S</sub></em><sub>2 </sub>is <em><sub>S</sub></em><sub>2_ </sub>= <em>{</em>2<em><sub>,</sub></em>1<em><sub>,</sub></em>4<em><sub>,</sub></em>9<em><sub>,</sub></em>14<em><sub>,</sub></em>13<em><sub>,</sub></em>16<em><sub>,</sub></em><strong><sub>18</sub></strong><em>} </em>Note that <em><sub>S</sub></em><sub>2_ </sub>contains node <strong><sub>18</sub></strong>, which means that the prefix “aa” is a matching prefix.

<ol start="4">
<li>Consuming b</li>
</ol>
The set of states that can be reached by consuming b starting from <em><sub>S</sub></em><sub>2_ </sub>is <em><sub>S</sub></em><sub>3 </sub>= <em><sub>{</sub></em>10<em><sub>}</sub></em>

The set of states that can be reached by consuming no input starting from <em><sub>S</sub></em><sub>3 </sub>is <em><sub>S</sub></em><sub>3_ </sub>= <em><sub>{</sub></em>10<em><sub>,</sub></em>11<em><sub>}</sub></em>

Note that <em><sub>S</sub></em><sub>3_ </sub>does not contain node <strong><sub>18 </sub></strong>which means that “aab” is not a matching prefix, but is still a viable prefix.

<ol start="5">
<li>Consuming a</li>
</ol>
The set of states that can be reached by consuming a starting from <em><sub>S</sub></em><sub>3_ </sub>is <em><sub>S</sub></em><sub>4 </sub>= <em>{} </em>Since <em><sub>S</sub></em><sub>4 </sub>is empty, “aaba” is not viable and we stop.

The longest matching prefix is aa. This is the lexeme that is returned. Note that the second call to match(r,s,p) starting after “aa” will return ERROR.

<h1>Instructions</h1>
Follow these steps:

<ul>
<li>Download the lexer.cc, lexer.h, inputbuf.cc and inputbuf.h files accompanying this project description. Note that these files might be a little different from the code you’ve seen in class or elsewhere.</li>
<li>Compile your code using GCC version 4.8.5 compiler on CentOS 7. You will need to use the g++ command to compile your code in a terminal window. See section 4 for more details on how to compile using GCC.</li>
</ul>
<strong>Note that you are required to compile and test your code on CentOS 7 using the GCC compiler version 4.8.5. </strong>You are free to use any IDE or text editor on any platform, however, using tools available in CentOS (or tools that you could install on CentOS) could save time in the development/compile/test cycle.

<ul>
<li>Test your code to see if it passes the provided test cases. You will need to extract the test cases from the zip file and run the test script test1.sh. See section 5 for more details.</li>
<li>Submit your code on the course submission website before the deadline. You can submit as many times as you need. Make sure your code is compiled correctly on the website, if you get a compiler error, fix the problem and submit again.</li>
<li><strong>Only the last version you submit is graded. There are no exception to this.</strong></li>
</ul>
<h2>Keep in mind that</h2>
<ul>
<li>You should use C/C++, no other programming languages are allowed.</li>
<li>All programming assignments in this course are individual assignments. Students must complete the assignments on their own.</li>
<li>You should submit your code on the course submission website, no other submission forms will be accepted.</li>
<li>You should familiarize yourself with the CentOS environment and the GCC compiler. Programming assignments in this course might be very different from what you are used to in other classes.</li>
</ul>
<h2>3. Evaluation</h2>
The submissions are evaluated based on the automated test cases on the submission website. Your grade will be proportional to the number of test cases passing. If your code does not compile on the submission website, you will not receive any points.

<strong>NOTE: The next two sections apply to all programming assignments.</strong>

You should use the instructions in the following sections to compile and test your programs for all programming assignments in this course.

<h2>4. Compiling your code with GCC</h2>
You should compile your programs with the GCC compilers which are available in CentOS 7. GCC is a collection of compilers for many programming languages. There are separate commands for compiling C and C++ programs:

<ul>
<li>Use the gcc command to compile C programs</li>
<li>Use the g++ command to compile C++ programs Here is an example of how to compile a simple C++ program:</li>
</ul>
$ g++ test_program.cpp

If the compilation is successful, it will generate an executable file named a.out in the same folder as the program. You can change the output file name by specifying the -o option:

$ g++ test_program.cpp -o hello.out

To enable C++11 with g++, use the -std=c++11 option:

$ g++ -std=c++11 test_program.cpp -o hello.out

The following table summarizes some useful GCC compiler options:

<table width="488">
<tbody>
<tr>
<td width="86">Switch</td>
<td width="118">Can be used with</td>
<td width="284">Description</td>
</tr>
<tr>
<td width="86">-o path</td>
<td width="118">gcc, g++</td>
<td width="284">Change the filename of the generated artifact</td>
</tr>
<tr>
<td width="86">-g</td>
<td width="118">gcc, g++</td>
<td width="284">Generate debugging information</td>
</tr>
<tr>
<td width="86">-ggdb</td>
<td width="118">gcc, g++</td>
<td width="284">Generate debugging information for use by GDB</td>
</tr>
<tr>
<td width="86">-Wall</td>
<td width="118">gcc, g++</td>
<td width="284">Enable most warning messages</td>
</tr>
<tr>
<td width="86">-w</td>
<td width="118">gcc, g++</td>
<td width="284">Inhibit all warning messages</td>
</tr>
<tr>
<td colspan="2" width="204">-std=c++11 g++</td>
<td width="284">Compile C++ code using 2011 C++ standard</td>
</tr>
<tr>
<td colspan="2" width="204">-std=c99&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; gcc</td>
<td width="284">Compile C code using ISO C99 standard</td>
</tr>
<tr>
<td colspan="2" width="204">-std=c11&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; gcc</td>
<td width="284">Compile C code using ISO C11 standard</td>
</tr>
</tbody>
</table>
You can find a comprehensive list of GCC options in the following page:

<a href="https://gcc.gnu.org/onlinedocs/gcc-4.8.5/gcc/">https://gcc.gnu.org/onlinedocs/gcc-4.8.5/gcc/</a>

<h2>Compiling projects with multiple files</h2>
If your program is written in multiple source files that should be linked together, you can compile and link all files together with one command:

$ g++ file1.cpp file2.cpp file3.cpp

Or you can compile them separately and then link:

$ g++ -c file1.cpp $ g++ -c file2.cpp $ g++ -c file3.cpp

$ g++ file1.o file2.o file3.o

The files with the .o extension are object files but are not executable. They are linked together with the last statement and the final executable will be a.out.

You can replace g++ with gcc in all examples listed above to compile C programs.

<h2>5. Testing your code on CentOS</h2>
Your programs should not explicitly open any file. You can only use the <strong><sub>standard input </sub></strong>e.g. std::cin in C++, getchar(), scanf() in C and <strong><sub>standard output </sub></strong>e.g. std::cout in C++, putchar(), printf() in C for input/output.

However, this restriction does not limit our ability to feed input to the program from files nor does it mean that we cannot save the output of the program in a file. We use a technique called standard IO redirection to achieve this.

Suppose we have an executable program a.out, we can run it by issuing the following command in a terminal (the dollar sign is not part of the command):

$ ./a.out

If the program expects any input, it waits for it to be typed on the keyboard and any output generated by the program will be displayed on the terminal screen.

To feed input to the program from a file, we can redirect the standard input to a file:

$ ./a.out &lt; input_data.txt

Now, the program will not wait for keyboard input, but rather read its input from the specified file. We can redirect the output of the program as well:

$ ./a.out &gt; output_file.txt

In this way, no output will be shown in the terminal window, but rather it will be saved to the specified file.

Note that programs have access to another standard stream which is called standard error e.g. std::cerr in C++, fprintf(stderr, …) in C. Any such output is still displayed on the terminal screen. It is possible to redirect standard error to a file as well, but we will not discuss that here. Finally, it’s possible to mix both into one command:

$ ./a.out &lt; input_data.txt &gt; output_file.txt

Which will redirect standard input and standard output to input_data.txt and output_file.txt respectively.

Now that we know how to use standard IO redirection, we are ready to test the program with test cases.

<h2>Test Cases</h2>
A test case is an input and output specification. For a given input there is an <em><sub>expected </sub></em>output. A test case for our purposes is usually represented by two files:

<ul>
<li>txt</li>
<li>txt.expected</li>
</ul>
The input is given in test_name.txt and the expected output is given in test_name.txt.expected. To test a program against a single test case, first we execute the program with the test input data:

$ ./a.out &lt; test_name.txt &gt; program_output.txt

The output generated by the program will be stored in program_output.txt. To see if the program generated the expected output, we need to compare program_output.txt and test_name.txt.expected. We do that using a general purpose tool called diff:

$ diff -Bw program_output.txt test_name.txt.expected

The options -Bw tell diff to ignore whitespace differences between the two files. If the files are the same

(ignoring the whitespace differences), we should see no output from diff, otherwise, diff will produce a report showing the differences between the two files.

We would simply consider the test <strong><sub>passed </sub></strong>if diff could not find any differences, otherwise we consider the test <strong>failed</strong>.

Our grading system uses this method to test your submissions against multiple test cases. There is also a test script accompanying this project test1.sh which will make your life easier by testing your code against multiple test cases with one command.

Here is how to use test1.sh to test your program:

<ul>
<li>Store the provided test cases zip file in the same folder as your project source files</li>
<li>Open a terminal window and navigate to your project folder</li>
<li>Unzip the test archive using the unzip command: bash $ unzip test_cases.zip</li>
</ul>
<strong>NOTE: </strong>the actual file name is probably different, you should replace test_cases.zip with the correct file name.

<ul>
<li>Store the test1.sh script in your project directory as well</li>
<li>Make the script executable: bash $ chmod +x test1.sh</li>
<li>Compile your program. The test script assumes your executable is called a.out</li>
<li>Run the script to test your code: bash $ ./test1.sh</li>
</ul>
The output of the script should be self explanatory. To test your code after you make changes, you will just perform the last two steps (compile and run test1.sh).

<a href="#_ftnref1" name="_ftn1">[1]</a> The graph is a representation of a non-deterministic finite state automaton
