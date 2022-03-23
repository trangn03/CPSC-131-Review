1. Suppose we have a proper Stack ADT. Where can you access and modify elements: the top

2. Suppose we would like to implement a Stack by re-using an existing container. Our Stack will be a wrapper (Adapter) over the other container and will simply call on that container's methods, so we don't have to write everything from scratch.

Going strictly by Big-O complexity classes, which container seems the best choice to wrap: list

Considering amortized analysis, which container is likely to perform better if we run benchmark tests: vector

3. Suppose we'd like to make a Stack by using the Adapter pattern with a different underlying container. For each container, name the position of that container that we should consider to be the Stack's top, to achieve the best efficiency.

Singly-Linked List: front

Doubly-Linked List: Front or back

Vector: anywhere 


4. Suppose we have the following stack:

s = [8,10,12,30,4]
For this question, assume the top of the stack is on the left side. Also assume that pop() would return the popped value (even though this is not always the case).

Now suppose we perform the following operations on the stack:

a = s.pop();
b = s.pop();
push(33);
push(82);
c = s.pop();
d = s.pop();
e = s.pop();
What is the final state of the stack? Use the exact format as above (no spaces, comma delimiters, and surround with brackets): [30,4]

What is the value of a: 8

What is the value of b: 10

What is the value of c: 82

What is the value of d: 33

What is the value of e: 12