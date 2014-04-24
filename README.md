Formal-Languages-And-Compilers
==============================

Lesson notes of Formal Languages and Compilers course @ UNITN

Syllabus
--------

INTRODUCTION
* Motivations and contents;
* Compilation break-down.

GRAMMARS
* Definitions and examples;
* Context-dependent vs context-free;
* Derivation trees;
* Ambiguous grammars

LEXING
* Regular expressions: Definition, shorthands, examples.
* NFA and DFA: Definitions; examples; Thompson's construction
* Subset construction: algorithm and examples
* DFA minimization: algorithm and examples
* Regular grammars and NFAs;
* Space/Time complexity of NFAs/DFAs;
* Not every language is regular;
* Pumping lemma for regular languages: proof, how-to, examples of application
* Lexemes, tokens, lexers; FLEX, JFlex

PARSING
* Introduction to parsing;
* Top-down parsing;
* Algorithm for predictive top-down parsing
* Definition of FIRST(X) and FOLLOW(A);
* Algorithm for the generation of predictive top-down parsing tables;
* LL(1) grammars
* Algorithmic definition of FIRST(alpha) and FOLLOW(A);
* LL(1) grammars: ambiguity, left recursion, left factoring.
* Elimination of left recursion.
* Left factorization.
* Bottom-up parsing: Shift/Reduce technique;
* LR parsing procedure;
* Collection of set of LR(0) items;
* Generation of SLR parsing table
* Associativity and precendence in SLR grammars;
* Conflict diagnosis for ambiguous grammars: case of E -> E+E | Ö
* LALR parsing: motivations; LR(1) items; adapted closure; adapted goto; lookahead propagation and generation from (I,j)
* Efficient computation of LALR parsing tables;
* Detailed example on the simple motivating grammar;
* SLR, LALR, and canonical LR parsing of the grammar for pointers

SYNTAX DIRECTED DEFINITIONS
* Synthesized attributes;
* Inherited attributes;
* Dependency graphs
* Controlled side effects: Typed lists of identifiers;
* S-attributed definition of abstract syntax trees;
* L-attributed definition of abstract syntax trees.
* Forcing semantic actions at appropriate time - the digit to numbers case;
* Production cloning;
* Unit and epsilon productions + global variables;
* Aggressive restructuring.

SYNTAX DIRECTED TRANSLATIONS AND INTERMEDIATE CODE GENERATION
* Syntax Directed Translations: Evaluation by preorder traversal of an enriched version of the parse tree;
* Use in the evaluation of inherited attributes during bottom-up parsing through markers and suitable grammar restructuring
* Three-address code representations;
* Code for basic and compound types (type expression and width).
* Control flow statements: if-then and side-effects in Java (example);
* Short-circuit code for boolean expressions;
* Control-flow translation of if-then and boolean expressions
* Cons of the easiest translation of boolean expressions, if-then, and while statements: redundant gotos and two-pass evaluation.
* Backpatching technique.
* Assignment and expressions in scope;
* Declarations and scoping; Observations on run-time environment.
* Yacc: guidelines and examples.
