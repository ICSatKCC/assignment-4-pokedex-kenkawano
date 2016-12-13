## Pokedex BST

### 68/100
Your basic binary search tree of Pokemon does work, but much of that code was given to you. The things that 
are extra to the PokeTree are mostly not working. You needed to give yourself more time and come ask me for help 
if you were stuck!

* Number caught cannot increment because increaseNumCaught( ) and decreaseNumCaught( ) in PokeNode are broken, 
they both check for num to be greater than 1 not less(-10)
* Pokenode constructor supposed to take in 4 parameters, takes 3 (no count) This was in the JUnit test!(-2)
* Pokenode throws PokeTreeExceptions rather than PokeNodeException 

* InOrder print method not in order, prints preorder (-10)
* Main method crashes when PokeTree correctly throws an exception, trying to remove a Pokemon not in the tree (-5)
* No Javadoc comments in any files. (-5)

----
### Pokedex Driver
- [ ] Catch Pokemon
 *  Add new Pokemon to the BST *This works*
 *  Increase the count of number caught of a Pokemon already in the tree.
- [ ] Trade Pokemon
 * Lower the quantity of a caught Pokemon in the BST.
 * Caught quantity cannot become negative.
 * Remove Pokemon from the tree that are all traded away. *This works*
*Crashes if you try to trade a Pokemon not in the tree. Tree correctly throws exception, but driver program doesn't catch it*
- [x]  Print out the Pokedex
*Prints in preOrder not inorder as assigned.*

- [ ] Commenting and coding style
 * No Javadoc

### PokeNode
- [x]  Node constructor
 *  Pokemon should be a non-null object.
 *  numCaught should be >= 1.
 * lChild and rChild are PokeNodes.

- [X]  Get methods
- []  Set methods
 * increaseNumCaught( )
 * decreaseNumCaught( )
   * broken checks for num greater than 1 rather than less.
   
 * no (or private) setPokemon method (okay for private PokeTree remove). 
- [ ] Commenting and coding style
 * No Javadoc

### PokeTree.java
- [x] Constructor:
- [x] public/private add methods
- [ ] public/private remove methods
 * decrements numCaught *Doesn't work because of PokeNode*
 * Removes Pokemon p from the tree if numCaught == 0
 * Throws exception if p not in the tree
- [x] Getting Pokemon in Tree by number:
 * public/private get methods
 * throws exception if Pokemon not in the tree
- [ ] Inorder traversal print method
- [ ] Commenting and coding style
 * No Javadoc
------
