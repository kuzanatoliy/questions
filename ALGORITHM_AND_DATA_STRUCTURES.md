# Algorithm and Data Structures

### Links

### Questions

<details>
  <summary>What is Algorithm?</summary>

An algorithm is an instruction that describes the order in which actions are to be performed. Algorithms describe how we transform data to get the desired result.

</details>

<details>
  <summary>What is Data Structure?</summary>

A data structure is a software unit that allows storing and processing data of the same type and/or logically related data.

</details>

<details>
  <summary>What is time complexity?</summary>

In general, the complexity is estimated as follows:
First, determine what blocks, independent in terms of operations, the program consists of. Calculate the execution time for each. The resulting time will be the maximum of these values.
For a block, count the number of operations of different types and the cost of each type of operation. The cost is clear: as a rule, it depends on the data structures with which the interaction takes place.

</details>

<details>
  <summary>What is off-by-one error?</summary>

It is error in index (+1). It could happen:

- during calculation of the array index
- if mix strong and not strong comparison

</details>

<details>
  <summary>What is binary search?</summary>

Binary search, also known as half-interval search, logarithmic search, or binary chop, is a search algorithm that finds the position of a target value within a sorted array.

</details>

<details>
  <summary>What is recursion?</summary>

Recursion is when a function calls itself. Recursion is not a specific algorithm, but a technique that allows algorithms to be implemented.

</details>

<details>
  <summary>What is divide and conquer method?</summary>

It is possible to provide follow work flow:

1. The source data is divided into several parts.
2. For each part, the function is called recursively.
3. The results of recursive calls are merged.

</details>

<details>
  <summary>What is Insertion sort?</summary>

Insertion sort is a simple sorting algorithm that builds the final sorted array (or list) one item at a time.

</details>

<details>
  <summary>What is Bubble sort?</summary>

Bubble sort, sometimes referred to as sinking sort, is a simple sorting algorithm that repeatedly steps through the input list element by element, comparing the current element with the one after it, swapping their values if needed. These passes through the list are repeated until no swaps had to be performed during a pass, meaning that the list has become fully sorted. The algorithm, which is a comparison sort, is named for the way the larger elements "bubble" up to the top of the list.

</details>

<details>
  <summary>What is Cocktail sort?</summary>

Cocktail shaker sort, also known as bidirectional bubble sort, cocktail sort, shaker sort (which can also refer to a variant of selection sort), ripple sort, shuffle sort, or shuttle sort, is an extension of bubble sort. The algorithm extends bubble sort by operating in two directions. While it improves on bubble sort by more quickly moving items to the beginning of the list, it provides only marginal performance improvements.

</details>

<details>
  <summary>What is Comb sort?</summary>

Comb sort is a relatively simple sorting algorithm originally designed by Włodzimierz Dobosiewicz and Artur Borowy in 1980, later rediscovered (and given the name "Combsort") by Stephen Lacey and Richard Box in 1991. Comb sort improves on bubble sort in the same way that Shellsort improves on insertion sort.

</details>

<details>
  <summary>What is Quick sort?</summary>

Quicksort is an in-place sorting algorithm. Developed by British computer scientist Tony Hoare in 1959 and published in 1961, it is still a commonly used algorithm for sorting. When implemented well, it can be somewhat faster than merge sort and about two or three times faster than heapsort.

</details>

<details>
  <summary>What is Merge sort?</summary>

Merge is an efficient, general-purpose, and comparison-based sorting algorithm. Most implementations produce a stable sort, which means that the order of equal elements is the same in the input and output.

</details>

<details>
  <summary>What is Heap sort?</summary>

In computer science, heapsort is a comparison-based sorting algorithm. Heapsort can be thought of as an improved selection sort: like selection sort, heapsort divides its input into a sorted and an unsorted region, and it iteratively shrinks the unsorted region by extracting the largest element from it and inserting it into the sorted region. Unlike selection sort, heapsort does not waste time with a linear-time scan of the unsorted region; rather, heap sort maintains the unsorted region in a heap data structure to more quickly find the largest element in each step.

</details>

<details>
  <summary>What types of graphs do you know?</summary>

- By the presence of direction: directed and not directed
- By the presence of scales: weighted and unweighted
- By the presence of cycles: cyclic and acyclic

</details>

<details>
  <summary>What ways of bypassing trees are?</summary>

- Preorder: visit the current node first, then look at its subtrees.
- Inorder: look at the left subtree, visit the current node, and then look at the right subtree. Applicable only to binary trees.
- Postorder: Consider all subtrees of the current node, then visit it.

</details>

<details>
  <summary>What is dynamic programming?</summary>

Dynamic programming is not a specific algorithm, but a technique that allows you to quickly solve a fairly wide class of problems. These questions often come up in interviews. In this tutorial we have chosen:

- about the basic idea of dynamic programming,
- about the types of tasks in interviews.

</details>

<details>
  <summary>What is greedy algorithm?</summary>

A greedy algorithm is one in which a locally optimal solution is chosen at each step.

</details>

<details>
  <summary>What are implementation tasks?</summary>

Implementation tasks are not algorithms in the usual sense, but they are common, so we also need to talk about them.

</details>

<details>
  <summary>What is dynamic array?</summary>

A dynamic array is the simplest data structure. It performs the same tasks as ordinary arrays, only it allows you to change its size at runtime.

</details>

<details>
  <summary>What is stack?</summary>

A stack is a data structure that allows you to quickly add an element to the end and quickly get the last element. In general, other operations may either not be supported or performed inefficiently.

</details>

<details>
  <summary>What is queue?</summary>

In computer science, a queue is a collection of entities that are maintained in a sequence and can be modified by the addition of entities at one end of the sequence and the removal of entities from the other end of the sequence. By convention, the end of the sequence at which elements are added is called the back, tail, or rear of the queue, and the end at which elements are removed is called the head or front of the queue, analogously to the words used when people line up to wait for goods or services.

</details>

<details>
  <summary>What is Linked list?</summary>

In computer science, a linked list is a linear collection of data elements whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of nodes which together represent a sequence. In its most basic form, each node contains: data, and a reference (in other words, a link) to the next node in the sequence. This structure allows for efficient insertion or removal of elements from any position in the sequence during iteration. More complex variants add additional links, allowing more efficient insertion or removal of nodes at arbitrary positions.

</details>

<details>
  <summary>What is hash table?</summary>

A hash table is a lookup data structure. It allows you to quickly add, search, and remove items. Based on it, the set and dictionary containers are implemented.

</details>
