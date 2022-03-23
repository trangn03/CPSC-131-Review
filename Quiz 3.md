1. Suppose we have the following code:

std::vector<int> v = {1, 2, 3, 4, 5, 6, 7};
for ( auto a : v ) {
  std::cout << a << std::endl;
}
We know the above range-based for loop will silently expand (under the hood) to something like the following:

for ( auto itr = BLANK1; itr != BLANK2; BLANK3 ) {
  auto a = BLANK4;
  std::cout << a << std::endl;
}
Now, fill in the omitted parts above. Do not use spaces in your answer.

BLANK1: v.begin()

BLANK2: v.end()

BLANK3: ++itr

BLANK4: *itr

2. One condition required for your custom class to be considered a Container, is it must support Iterators / Iteration : True

3. Suppose we have two iterators: itr1 and itr2.

Suppose itr1 refers to a singly-linked list, and itr2 refers to a doubly-linked list. Answer the following questions for these two iterators, from the perspective of Big-O complexity classes (not exact measurements).

Which of the two iterators is faster while stepping forward through the container (assume we have forward iterators): About the same

Which of the two iterators is faster while stepping backward through the container (assume we have reverse iterators): itr2

What is the time complexity of itr1 while stepping forward: O[1]

What is the time complexity of itr2 while stepping forward: O[1]

What is the time complexity of itr1 while stepping backward: O[n]

What is the time complexity of itr2 while stepping backward: O[1]

4. Suppose we have the following vector containing dog names:
std::vector<std::string> v = {"Bacon", "Taco", "Barkley", "Subwoofer", "Chewie", "Einstein", "Slink", "Waldo"};
Now, suppose that for each code snippet below, we first start by initializing an iterator with the following:

auto itr = v.begin();
(suppose we do this before EACH snippet, so all snippets start at the beginning)

Examine each code snippet and decide where the iterator would point after the snippet executes. Select the std::string to indicate the iterator's new position. Note that some snippets have 2 statements.

itr += 0: Bacon
itr++: Taco
itr += 3; itr -=1: Barkley
itr += 3; ++itr: Chewie

5. Suppose we have a random access iterator itr.

For each type of container below, name the efficiency class of an operation performed with the iterator. Don't assume steps in any direction, or any amount. Assume "moving" means "moving to any arbitrary position in the container".

Vector
Moving: O[1]
Accessing the current element: O[1]

Singly Linked List
Moving: O[n]
Accessing the current element: O[1]

Doubly Linked List
Moving: O[n]
Accessing the current element: O[1]
