
DevNote: Java Inside
==================

### static Block
The code block with the static modifier signifies a class initializer; without the static modifier the code block is an instance initializer.

Class initializers are executed in the order they are defined (top down, just like simple variable initializers) when the class is loaded (actually, when it's resolved, but that's a technicality).

Instance initializers are executed in the order defined when the class is instantiated, immediately before the constructor code is executed, immediately after the invocation of the super constructor.

If you remove static from int a, it becomes an instance variable which is not initialized at construction. If you also remove static from the initializer block, it then becomes an instance initializer and so int a is initialized at construction.

> Written with [StackEdit](https://stackedit.io/).