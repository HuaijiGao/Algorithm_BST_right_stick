# Algorithm_BST_right_stick

# scenario
You are a hacker that recently got hired by a cybersecurity company. The team needs to be preemptive
against any adversarial attacks. Your role is to develop such attacks so the defense team can prepare
mechanisms to avoid them.

In this problem, you were able to inject code into the algorithm for inserting an element into a Binary
Search Tree. Your goal is to force the BST to always degrade to a ”stick” (to the right), or
more specifically, a linked list. The algorithm to insert an element into the BST is as follows.

<img width="456" alt="image" src="https://user-images.githubusercontent.com/19381768/197389813-a925cca4-2b06-4f86-bbe0-6ac51b1ac292.png">

Here root and new are nodes with fields left and right (which are pointers to other nodes) and a field
value. If the BST is already a ”right stick”, then running the BSTInsert algorithm (with your Stickify
function) should always leave the tree as a ”right stick”.

For example if we start with the tree on the left and insert 2 we will get the tree in the middle. After
Stickify is run, we should get the tree on the right.

<img width="931" alt="image" src="https://user-images.githubusercontent.com/19381768/197389831-ace7cd02-e4e1-46cc-8334-fac808bf1677.png">

Your task is to write the pseudocode for the algorithm Stickify which takes the newly inserted node
along with its parent and performs any necessary rotations to ensure the tree remains a ”right stick”.
You may use RotateRight(node) and RotateLeft(node) without implementing these functions. In
the above example, the RotateRight(3) should be called.
