BooleanBackpatch:

For the given boolean expression truelist and falselist are generated.

ControlFlowGraph(CFG):

For the given block of statement, three address statement,basic block and control flow graph are generated.

If-Else:

Add the "else" statement for the corresponding "if" statement.

For-While:

For the given "for" statement has been converted into "while" statement.

SyntaxTree:

For the given arthimetic expression  the syntax tree is generated.

SymbolTable:

For the given set of declaration statement the symbol table is generated.

ConstantPropogation:

For the given block of statements, three address code,basic block,DAG are generated.If constant folding occurs,new three address code is generated.

LabeledTree:

For the given arithemetic expression, labeled tree is generated.
  
  
How to compile:

open the terminal

lex filename.l

yacc -d filename.l
  
  if-else,for-while,Syntax tree,Symbol table:

gcc lex.yy.c y.tab.c -ll 

./a.out
  
  Boolean backpatch,CFG,ConstantPropogation,Labeledtree:

g++ lex.yy.c y.tab.c -lfl 

./a.out<inputtextfile
  
  
