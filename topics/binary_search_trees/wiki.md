The following text has been accessed from https://en.wikipedia.org/wiki/Binary_search_tree at Fri Aug 9 01:08:06 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Binary search tree ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Binary search tree
Type        tree
Invented    1960
Invented by P.F. Windley, A.D._Booth, A.J.T._Colin, and T.N._Hibbard
Time_complexity in big_O_notation
Algorithm  Average  Worst case
Space      O(n)     O(n)
Search     O(log n) O(n)
Insert     O(log n) O(n)
Delete     O(log n) O(n)
A binary search tree of size 9 and depth 3, with 8 at the root. The leaves are
not drawn.
In computer_science, binary search trees (BST), sometimes called ordered or
sorted binary trees, are a particular type of container: a data_structure that
stores "items" (such as numbers, names etc.) in memory. They allow fast lookup,
addition and removal of items, and can be used to implement either dynamic_sets
of items, or lookup_tables that allow finding an item by its key (e.g., finding
the phone number of a person by name).
Binary search trees keep their keys in sorted order, so that lookup and other
operations can use the principle of binary_search: when looking for a key in a
tree (or a place to insert a new key), they traverse the tree from root to
leaf, making comparisons to keys stored in the nodes of the tree and deciding,
on the basis of the comparison, to continue searching in the left or right
subtrees. On average, this means that each comparison allows the operations to
skip about half of the tree, so that each lookup, insertion or deletion takes
time_proportional_to the logarithm of the number of items stored in the tree.
This is much better than the linear_time required to find items by key in an
(unsorted) array, but slower than the corresponding operations on hash_tables.
Several variants of the binary search tree have been studied in computer
science; this article deals primarily with the basic type, making references to
more advanced types when appropriate.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Order_relation
    * 2_Operations
          o 2.1_Searching
          o 2.2_Insertion
          o 2.3_Deletion
          o 2.4_Traversal
          o 2.5_Verification
    * 3_Examples_of_applications
          o 3.1_Sort
          o 3.2_Priority_queue_operations
    * 4_Types
          o 4.1_Performance_comparisons
          o 4.2_Optimal_binary_search_trees
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Definition[edit] *****
A binary search tree is a rooted binary_tree, whose internal nodes each store a
key (and optionally, an associated value) and each have two distinguished sub-
trees, commonly denoted left and right. The tree additionally satisfies the
binary_search property, which states that the key in each node must be greater
than or equal to any key stored in the left sub-tree, and less than or equal to
any key stored in the right sub-tree.[1]:287 The leaves (final nodes) of the
tree contain no key and have no structure to distinguish them from one another.
Frequently, the information represented by each node is a record rather than a
single data element. However, for sequencing purposes, nodes are compared
according to their keys rather than any part of their associated records. The
major advantage of binary search trees over other data structures is that the
related sorting_algorithms and search_algorithms such as in-order_traversal can
be very efficient; they are also easy to code.
Binary search trees are a fundamental data structure used to construct more
abstract data structures such as sets, multisets, and associative_arrays.
    * When inserting or searching for an element in a binary search tree, the
      key of each visited node has to be compared with the key of the element
      to be inserted or found.
    * The shape of the binary search tree depends entirely on the order of
      insertions and deletions, and can become degenerate.
    * After a long intermixed sequence of random insertion and deletion, the
      expected height of the tree approaches square root of the number of keys,
      √n, which grows much faster than log n.
    * There has been a lot of research to prevent degeneration of the tree
      resulting in worst case time complexity of O(n) (for details see section
      Types).
**** Order relation[edit] ****
Binary search requires an order relation by which every element (item) can be
compared with every other element in the sense of a total_preorder. The part of
the element which effectively takes place in the comparison is called its key.
Whether duplicates, i.e. different elements with same key, shall be allowed in
the tree or not, does not depend on the order relation, but on the application
only.
In the context of binary search trees a total preorder is realized most
flexibly by means of a three-way_comparison subroutine.
***** Operations[edit] *****
Binary search trees support three main operations: insertion of elements,
deletion of elements, and lookup (checking whether a key is present).
**** Searching[edit] ****
Searching a binary search tree for a specific key can be programmed recursively
or iteratively.
We begin by examining the root_node. If the tree is null, the key we are
searching for does not exist in the tree. Otherwise, if the key equals that of
the root, the search is successful and we return the node. If the key is less
than that of the root, we search the left subtree. Similarly, if the key is
greater than that of the root, we search the right subtree. This process is
repeated until the key is found or the remaining subtree is null. If the
searched key is not found after a null subtree is reached, then the key is not
present in the tree. This is easily expressed as a recursive algorithm
(implemented in Python):
1 def search_recursively(key, node):
2     if node is None or node.key == key:
3         return node
4     if key < node.key:
5         return search_recursively(key, node.left)
6     # key > node.key
7     return search_recursively(key, node.right)
The same algorithm can be implemented iteratively:
 1 def search_iteratively(key, node):
 2     current_node = node
 3     while current_node is not None:
 4         if key == current_node.key:
 5             return current_node
 6         if key < current_node.key:
 7             current_node = current_node.left
 8         else: # key > current_node.key:
 9             current_node = current_node.right
10     return current_node
These two examples rely on the order relation being a total order.
If the order relation is only a total preorder, a reasonable extension of the
functionality is the following: also in case of equality search down to the
leaves in a direction specified by the user. A binary_tree_sort equipped with
such a comparison function becomes stable.
Because in the worst case this algorithm must search from the root of the tree
to the leaf farthest from the root, the search operation takes time
proportional to the tree's height (see tree_terminology). On average, binary
search trees with n nodes have O(log n) height.[note_1] However, in the worst
case, binary search trees can have O(n) height, when the unbalanced tree
resembles a linked_list (degenerate_tree).
**** Insertion[edit] ****
Insertion begins as a search would begin; if the key is not equal to that of
the root, we search the left or right subtrees as before. Eventually, we will
reach an external node and add the new key-value pair (here encoded as a record
'newNode') as its right or left child, depending on the node's key. In other
words, we examine the root and recursively insert the new node to the left
subtree if its key is less than that of the root, or the right subtree if its
key is greater than or equal to the root.
Here's how a typical binary search tree insertion might be performed in a
binary tree in C++:
void insert(Node*& root, int key, int value) {
  if (!root)
    root = new Node(key, value);
  else if (key == root->key)
    root->value = value;
  else if (key < root->key)
    insert(root->left, key, value);
  else  // key > root->key
    insert(root->right, key, value);
}
Alternatively, a non-recursive version might be implemented like this. Using a
pointer-to-pointer to keep track of where we came from lets the code avoid
explicit checking for and handling of the case where it needs to insert a node
at the tree root[2]:
void insert(Node** root, int key, int value) {
  Node **walk = root;
  while (*walk) {
    int curkey = (*walk)->key;
    if (curkey == key) {
      (*walk)->value = value;
      return;
    }
    if (key > curkey)
      walk = &(*walk)->right;
    else
      walk = &(*walk)->left;
  }
  *walk = new Node(key, value);
}
The above destructive procedural variant modifies the tree in place. It uses
only constant heap space (and the iterative version uses constant stack space
as well), but the prior version of the tree is lost. Alternatively, as in the
following Python example, we can reconstruct all ancestors of the inserted
node; any reference to the original tree root remains valid, making the tree a
persistent_data_structure:
def binary_tree_insert(node, key, value):
   if node is None:
       return NodeTree(None, key, value, None)
   if key == node.key:
       return NodeTree(node.left, key, value, node.right)
   if key < node.key:
       return NodeTree(binary_tree_insert(node.left, key, value), node.key,
node.value, node.right)
   return NodeTree(node.left, node.key, node.value, binary_tree_insert
(node.right, key, value))
The part that is rebuilt uses O(log n) space in the average case and O(n) in
the worst case.
In either version, this operation requires time proportional to the height of
the tree in the worst case, which is O(log n) time in the average case over all
trees, but O(n) time in the worst case.
Another way to explain insertion is that in order to insert a new node in the
tree, its key is first compared with that of the root. If its key is less than
the root's, it is then compared with the key of the root's left child. If its
key is greater, it is compared with the root's right child. This process
continues, until the new node is compared with a leaf node, and then it is
added as this node's right or left child, depending on its key: if the key is
less than the leaf's key, then it is inserted as the leaf's left child,
otherwise as the leaf's right child.
There are other ways of inserting nodes into a binary tree, but this is the
only way of inserting nodes at the leaves and at the same time preserving the
BST structure.
**** Deletion[edit] ****
When removing a node from a binary search tree it is mandatory to maintain the
in-order sequence of the nodes. There are many possibilities to do this.
However, the following method which has been proposed by T. Hibbard in 1962[3]
guarantees that the heights of the subject subtrees are changed by at most one.
There are three possible cases to consider:
    * Deleting a node with no children: simply remove the node from the tree.
    * Deleting a node with one child: remove the node and replace it with its
      child.
    * Deleting a node with two children: call the node to be deleted D. Do not
      delete D. Instead, choose either its in-order predecessor node or its in-
      order successor node as replacement node E (s. figure). Copy the user
      values of E to D.[note_2] If E does not have a child simply remove E from
      its previous parent G. If E has a child, say F, it is a right child.
      Replace E with F at E's parent.
Deleting a node with two children from a binary search tree. First the leftmost
node in the right subtree, the in-order successor E, is identified. Its value
is copied into the node D being deleted. The in-order successor can then be
easily deleted because it has at most one child. The same method works
symmetrically using the in-order predecessor C.
In all cases, when D happens to be the root, make the replacement node root
again.
Broadly speaking, nodes with children are harder to delete. As with all binary
trees, a node's in-order successor is its right subtree's left-most child, and
a node's in-order predecessor is the left subtree's right-most child. In either
case, this node will have only one or no child at all. Delete it according to
one of the two simpler cases above.
Consistently using the in-order successor or the in-order predecessor for every
instance of the two-child case can lead to an unbalanced tree, so some
implementations select one or the other at different times.
Runtime analysis: Although this operation does not always traverse the tree
down to a leaf, this is always a possibility; thus in the worst case it
requires time proportional to the height of the tree. It does not require more
even when the node has two children, since it still follows a single path and
does not visit any node twice.
def find_min(self):   # Gets minimum node in a subtree
    current_node = self
    while current_node.left_child:
        current_node = current_node.left_child
    return current_node

def replace_node_in_parent(self, new_value=None):
    if self.parent:
        if self == self.parent.left_child:
            self.parent.left_child = new_value
        else:
            self.parent.right_child = new_value
    if new_value:
        new_value.parent = self.parent

def binary_tree_delete(self, key):
    if key < self.key:
        self.left_child.binary_tree_delete(key)
        return
    if key > self.key:
        self.right_child.binary_tree_delete(key)
        return
    # delete the key here
    if self.left_child and self.right_child: # if both children are present
        successor = self.right_child.find_min()
        self.key = successor.key
        successor.binary_tree_delete(successor.key)
    elif self.left_child:   # if the node has only a *left* child
        self.replace_node_in_parent(self.left_child)
    elif self.right_child:  # if the node has only a *right* child
        self.replace_node_in_parent(self.right_child)
    else:
        self.replace_node_in_parent(None) # this node has no children
**** Traversal[edit] ****
Main article: Tree_traversal
Once the binary search tree has been created, its elements can be retrieved in-
order by recursively traversing the left subtree of the root node, accessing
the node itself, then recursively traversing the right subtree of the node,
continuing this pattern with each node in the tree as it's recursively
accessed. As with all binary trees, one may conduct a pre-order_traversal or a
post-order_traversal, but neither are likely to be useful for binary search
trees. An in-order traversal of a binary search tree will always result in a
sorted list of node items (numbers, strings or other comparable items).
The code for in-order traversal in Python is given below. It will call callback
(some function the programmer wishes to call on the node's value, such as
printing to the screen) for every node in the tree.
def traverse_binary_tree(node, callback):
    if node is None:
        return
    traverse_binary_tree(node.leftChild, callback)
    callback(node.value)
    traverse_binary_tree(node.rightChild, callback)
Traversal requires O(n) time, since it must visit every node. This algorithm is
also O(n), so it is asymptotically_optimal.
Traversal can also be implemented iteratively. For certain applications, e.g.
greater equal search, approximative search, an operation for single step
(iterative) traversal can be very useful. This is, of course, implemented
without the callback construct and takes O(1) on average and O(log n) in the
worst case.
**** Verification[edit] ****
Sometimes we already have a binary tree, and we need to determine whether it is
a BST. This problem has a simple recursive solution.
The BST propertyâevery node on the right subtree has to be larger than the
current node and every node on the left subtree has to be smaller than the
current nodeâis the key to figuring out whether a tree is a BST or not. The
greedy_algorithmâsimply traverse the tree, at every node check whether the
node contains a value larger than the value at the left child and smaller than
the value on the right childâdoes not work for all cases. Consider the
following tree:
     20
    /  \
  10    30
       /  \
      5    40
In the tree above, each node meets the condition that the node contains a value
larger than its left child and smaller than its right child hold, and yet it is
not a BST: the value 5 is on the right subtree of the node containing 20, a
violation of the BST property.
Instead of making a decision based solely on the values of a node and its
children, we also need information flowing down from the parent as well. In the
case of the tree above, if we could remember about the node containing the
value 20, we would see that the node with value 5 is violating the BST property
contract.
So the condition we need to check at each node is:
    * if the node is the left child of its parent, then it must be smaller than
      (or equal to) the parent and it must pass down the value from its parent
      to its right subtree to make sure none of the nodes in that subtree is
      greater than the parent
    * if the node is the right child of its parent, then it must be larger than
      the parent and it must pass down the value from its parent to its left
      subtree to make sure none of the nodes in that subtree is lesser than the
      parent.
A recursive solution in C++ can explain this further:
struct TreeNode {
    int key;
    int value;
    struct TreeNode *left;
    struct TreeNode *right;
};

bool isBST(struct TreeNode *node, int minKey, int maxKey) {
    if (node == NULL) return true;
    if (node->key < minKey || node->key > maxKey) return false;

    return isBST(node->left, minKey, node->key-1) && isBST(node->right, node-
>key+1, maxKey);
}
node->key+1 and node->key-1 are done to allow only distinct elements in BST.
If we want same elements to also be present, then we can use only node->key in
both places.
The initial call to this function can be something like this:
if (isBST(root, INT_MIN, INT_MAX)) {
    puts("This is a BST.");
} else {
    puts("This is NOT a BST!");
}
Essentially we keep creating a valid range (starting from [MIN_VALUE,
MAX_VALUE]) and keep shrinking it down for each node as we go down recursively.
As pointed out in section #Traversal, an in-order traversal of a binary search
tree returns the nodes sorted. Thus we only need to keep the last visited node
while traversing the tree and check whether its key is smaller (or smaller/
equal, if duplicates are to be allowed in the tree) compared to the current
key.
***** Examples of applications[edit] *****
**** Sort[edit] ****
Main article: Tree_sort
A binary search tree can be used to implement a simple sorting_algorithm.
Similar to heapsort, we insert all the values we wish to sort into a new
ordered data structureâin this case a binary search treeâand then traverse
it in order.
The worst-case time of build_binary_tree is O(n2)âif you feed it a sorted
list of values, it chains them into a linked_list with no left subtrees. For
example, build_binary_tree([1, 2, 3, 4, 5]) yields the tree (1 (2 (3 (4
(5))))).
There are several schemes for overcoming this flaw with simple binary trees;
the most common is the self-balancing_binary_search_tree. If this same
procedure is done using such a tree, the overall worst-case time is O(n log n),
which is asymptotically_optimal for a comparison_sort. In practice, the added
overhead in time and space for a tree-based sort (particularly for node
allocation) make it inferior to other asymptotically optimal sorts such as
heapsort for static list sorting. On the other hand, it is one of the most
efficient methods of incremental sorting, adding items to a list over time
while keeping the list sorted at all times.
**** Priority queue operations[edit] ****
Binary search trees can serve as priority_queues: structures that allow
insertion of arbitrary key as well as lookup and deletion of the minimum (or
maximum) key. Insertion works as previously explained. Find-min walks the tree,
following left pointers as far as it can without hitting a leaf:
// Precondition: T is not a leaf
function find-min(T):
    while hasLeft(T):
        T ? left(T)
    return key(T)
Find-max is analogous: follow right pointers as far as possible. Delete-min
(max) can simply look up the minimum (maximum), then delete it. This way,
insertion and deletion both take logarithmic time, just as they do in a binary
heap, but unlike a binary heap and most other priority queue implementations, a
single tree can support all of find-min, find-max, delete-min and delete-max at
the same time, making binary search trees suitable as double-ended_priority
queues.[4]:156
***** Types[edit] *****
There are many types of binary search trees. AVL_trees and red-black_trees are
both forms of self-balancing_binary_search_trees. A splay_tree is a binary
search tree that automatically moves frequently accessed elements nearer to the
root. In a treap (tree heap), each node also holds a (randomly chosen) priority
and the parent node has higher priority than its children. Tango_trees are
trees optimized for fast searches. T-trees are binary search trees optimized to
reduce storage space overhead, widely used for in-memory databases
A degenerate tree is a tree where for each parent node, there is only one
associated child node. It is unbalanced and, in the worst case, performance
degrades to that of a linked list. If your add node function does not handle
re-balancing, then you can easily construct a degenerate tree by feeding it
with data that is already sorted. What this means is that in a performance
measurement, the tree will essentially behave like a linked list data
structure.
**** Performance comparisons[edit] ****
D. A. Heger (2004)[5] presented a performance comparison of binary search
trees. Treap was found to have the best average performance, while red-black
tree was found to have the smallest number of performance variations.
**** Optimal binary search trees[edit] ****
Main article: Optimal_binary_search_tree
Tree rotations are very common internal operations in binary trees to keep
perfect, or near-to-perfect, internal balance in the tree.
If we do not plan on modifying a search tree, and we know exactly how often
each item will be accessed, we can construct[6] an optimal binary search tree,
which is a search tree where the average cost of looking up an item (the
expected search cost) is minimized.
Even if we only have estimates of the search costs, such a system can
considerably speed up lookups on average. For example, if you have a BST of
English words used in a spell_checker, you might balance the tree based on word
frequency in text_corpora, placing words like the near the root and words like
agerasia near the leaves. Such a tree might be compared with Huffman_trees,
which similarly seek to place frequently used items near the root in order to
produce a dense information encoding; however, Huffman trees store data
elements only in leaves, and these elements need not be ordered.
If we do not know the sequence in which the elements in the tree will be
accessed in advance, we can use splay_trees which are asymptotically as good as
any static search tree we can construct for any particular sequence of lookup
operations.
Alphabetic trees are Huffman trees with the additional constraint on order, or,
equivalently, search trees with the modification that all elements are stored
in the leaves. Faster algorithms exist for optimal alphabetic binary trees
(OABTs).
***** See also[edit] *****
    * Binary_search_algorithm
    * Search_tree
    * Self-balancing_binary_search_tree
    * AVL_tree
    * Redâblack_tree
    * Randomized_binary_search_tree
    * Tango_tree
***** Notes[edit] *****
   1. ^ The notion of an average BST is made precise as follows. Let a random
      BST be one built using only insertions out of a sequence of unique
      elements in random order (all permutations equally likely); then the
      expected height of the tree is O(log n). If deletions are allowed as well
      as insertions, "little is known about the average height of a binary
      search tree".[1]:300
   2. ^ Of course, a generic software package has to work the other way around:
      It has to leave the user data untouched and to furnish E with all the BST
      links to and from D.
***** References[edit] *****
   1. ^ a bCormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,
      Clifford (2009) [1990]. Introduction_to_Algorithms (3rd ed.). MIT Press
      and McGraw-Hill. ISBN 0-262-03384-4.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
      .citation q{quotes:"\"""\"""'""'"}.mw-parser-output .citation .cs1-lock-
      free a{background:url("//upload.wikimedia.org/wikipedia/commons/thumb/6/
      65/Lock-green.svg/9px-Lock-green.svg.png")no-repeat;background-position:
      right .1em center}.mw-parser-output .citation .cs1-lock-limited a,.mw-
      parser-output .citation .cs1-lock-registration a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Lock-gray-alt-2.svg/
      9px-Lock-gray-alt-2.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output .citation .cs1-lock-subscription a{background:
      url("//upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Lock-red-alt-
      2.svg/9px-Lock-red-alt-2.svg.png")no-repeat;background-position:right
      .1em center}.mw-parser-output .cs1-subscription,.mw-parser-output .cs1-
      registration{color:#555}.mw-parser-output .cs1-subscription span,.mw-
      parser-output .cs1-registration span{border-bottom:1px dotted;cursor:
      help}.mw-parser-output .cs1-ws-icon a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Wikisource-logo.svg/
      12px-Wikisource-logo.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output code.cs1-code{color:inherit;background:
      inherit;border:inherit;padding:inherit}.mw-parser-output .cs1-hidden-
      error{display:none;font-size:100%}.mw-parser-output .cs1-visible-error
      {font-size:100%}.mw-parser-output .cs1-maint{display:none;color:
      #33aa33;margin-left:0.3em}.mw-parser-output .cs1-subscription,.mw-parser-
      output .cs1-registration,.mw-parser-output .cs1-format{font-size:95%}.mw-
      parser-output .cs1-kern-left,.mw-parser-output .cs1-kern-wl-left{padding-
      left:0.2em}.mw-parser-output .cs1-kern-right,.mw-parser-output .cs1-kern-
      wl-right{padding-right:0.2em}
   3. ^Trubetskoy, Gregory. "Linus_on_understanding_pointers". Retrieved 21
      February 2019.
   4. ^ s. Robert_Sedgewick, Kevin Wayne: Algorithms_Fourth_Edition. Pearson
      Education, 2011,
   5. ISBN 978-0-321-57351-3, p. 410.
   6. ^Mehlhorn,_Kurt; Sanders,_Peter (2008). Algorithms_and_Data_Structures:
      The_Basic_Toolbox (PDF). Springer.
   7. ^Heger, Dominique A. (2004), "A_Disquisition_on_The_Performance_Behavior
      of_Binary_Search_Tree_Data_Structures" (PDF), European Journal for the
      Informatics Professional, 5 (5): 67â75
   8. ^Gonnet, Gaston. "Optimal_Binary_Search_Trees". Scientific Computation.
      ETH ZÃ¼rich. Archived from the_original on 12 October 2014. Retrieved 1
      December 2013.
***** Further reading[edit] *****
    *  This article incorporates public_domain_material from the NIST document:
       Black, Paul E. "Binary_Search_Tree". Dictionary_of_Algorithms_and_Data
      Structures.
Cormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,_Clifford
(2001). "12: Binary search trees, 15.5: Optimal binary search trees".
Introduction_to_Algorithms (2nd ed.). MIT Press & McGraw-Hill. pp. 253â272,
356â363. ISBN 0-262-03293-7.
Jarc, Duane J. (3 December 2005). "Binary_Tree_Traversals". Interactive Data
Structure Visualizations. University_of_Maryland.
Knuth,_Donald (1997). "6.2.2: Binary Tree Searching". The_Art_of_Computer
Programming. 3: "Sorting and Searching" (3rd ed.). Addison-Wesley.
pp. 426â458. ISBN 0-201-89685-0.
Long, Sean. "Binary_Search_Tree" (PPT). Data Structures and Algorithms
Visualization-A PowerPoint Slides Based Approach. SUNY_Oneonta.
Parlante, Nick (2001). "Binary_Trees". CS Education Library. Stanford
University.
***** External links[edit] *****
    * Binary_Tree_Visualizer (JavaScript animation of various BT-based data
      structures)
    * Kovac, Kubo. "Binary_Search_Trees" (Java_applet). KoreÅ¡ponden?nÃ½
      seminÃ¡r z programovania.
Madru, Justin (18 August 2009). "Binary_Search_Tree". JDServer. Archived from
the_original on 28 March 2010.
 C++ implementation.
Binary_Search_Tree_Example_in_Python
"References_to_Pointers_(C++)". MSDN. Microsoft. 2005.
 Gives an example binary tree implementation.
    * v
    * t
    * e
Tree_data_structures
                                      * 2â3
                                      * 2â3â4
                                      * AA
                                      * (a,b)
                                      * AVL
                                      * B
                                      * B+
                                      * B*
                                      * Bx
Search_trees                          * (Optimal) Binary search
(dynamic_sets/associative_arrays)     * Dancing
                                      * HTree
                                      * Interval
                                      * Order_statistic
                                      * (Left-leaning) Red-black
                                      * Scapegoat
                                      * Splay
                                      * T
                                      * Treap
                                      * UB
                                      * Weight-balanced
                                      * Binary
                                      * Binomial
                                      * Brodal
                                      * Fibonacci
Heaps                                 * Leftist
                                      * Pairing
                                      * Skew
                                      * van_Emde_Boas
                                      * Weak
                                      * Ctrie
                                      * C-trie_(compressed_ADT)
                                      * Hash
Tries                                 * Radix
                                      * Suffix
                                      * Ternary_search
                                      * X-fast
                                      * Y-fast
                                      * Ball
                                      * BK
                                      * BSP
                                      * Cartesian
                                      * Hilbert_R
                                      * k-d (implicit_k-d)
                                      * M
                                      * Metric
Spatial data partitioning trees       * MVP
                                      * Octree
                                      * Priority_R
                                      * Quad
                                      * R
                                      * R+
                                      * R*
                                      * Segment
                                      * VP
                                      * X
                                      * Cover
                                      * Exponential
                                      * Fenwick
                                      * Finger
                                      * Fractal_tree_index
                                      * Fusion
                                      * Hash_calendar
                                      * iDistance
Other trees                           * K-ary
                                      * Left-child_right-sibling
                                      * Link/cut
                                      * Log-structured_merge
                                      * Merkle
                                      * PQ
                                      * Range
                                      * SPQR
                                      * Top
    * v
    * t
    * e
Data_structures
Types        * Collection
             * Container
             * Associative_array
                   o Multimap
             * List
             * Stack
             * Queue
Abstract           o Double-ended_queue
             * Priority_queue
                   o Double-ended_priority_queue
             * Set
                   o Multiset
                   o Disjoint-set
             * Bit_array
             * Circular_buffer
Arrays       * Dynamic_array
             * Hash_table
             * Hashed_array_tree
             * Sparse_matrix
             * Association_list
             * Linked_list
Linked       * Skip_list
             * Unrolled_linked_list
             * XOR_linked_list
             * B-tree
             * Binary search tree
                   o AA_tree
                   o AVL_tree
                   o Redâblack_tree
                   o Self-balancing_tree
                   o Splay_tree
             * Heap
Trees              o Binary_heap
                   o Binomial_heap
                   o Fibonacci_heap
             * R-tree
                   o R*_tree
                   o R+_tree
                   o Hilbert_R-tree
             * Trie
                   o Hash_tree
             * Binary_decision_diagram
Graphs       * Directed_acyclic_graph
             * Directed_acyclic_word_graph
    * List_of_data_structures

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Binary_search_tree&oldid=897760028"
Categories:
    * Binary_trees
    * Data_types
    * Search_trees
Hidden categories:
    * CS1:_long_volume_value
    * Articles_with_example_C++_code
    * Articles_with_example_Python_code
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 19 May 2019, at 05:51 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
