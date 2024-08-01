# Natural numbers vs Even numbers

I would like to start with question - is there as many natural numbers as even numbers?
Intuition says no but let's check it.

What does it even mean that sets have the same size? Well, they have the same number of elements, right?
Example:
set A = {1,2,3}
set B = {5,6,8}

these are the same size. Both set A and set B have 3 elements.

That was easy because we could count number of elements. It's worse when we would like to count number of elements in infinite set.
You can think of the biggest number you can imagine and you can always add 1 to it. So it's impossible to count them in a way we did in first example.

There is another option, we can try to pair elements from both sets. If we go back to previous example we can see that all elements from set A have a pair in set B.
Pair for 1 from A will be 5 from B, pair for 2 from A will be 6 from B and pair for 3 from A will be 8 from B. 
Okay, we again showed that sets size are the same even though we didn't count them. 
Moreover, we created bijection between two sets. Bijection seems like something really tricky and hard in math but it's basically funtion one to one.
If you can find for every element from A corresponding element from B then it's bijection, if you can't it's not.


Let's switch to more interesting problem if we already have idea how to deal with it.
Again we have two sets:
N = {0, 1, 2, 3, 4, ...}
E = {0, 2, 4, 6, 8, ...}

If we were used our intuition we would say that set N is bigger because we have the same numbers plus something else e.g 3.
Yes but still there is no option to count it so let's try to use our second idea - let's pair them or find bijection as it's sound cooler.

For 0 from N we have 0 from E
for 1 from N we have 2 from E
for 2 from N we have 4 from E
...
for n from N we have 2N from E

we just showed that every element from N has corresponding element in E! All elements have a pair so size of N and E must be the same! 

Conclusion: **We have as many natural numbers as even numbers!**




https://math.stackexchange.com/questions/341605/as-many-even-numbers-as-natural-numbers
https://en.wikipedia.org/wiki/Bijection#:~:text=A%20bijection%2C%20bijective%20function%2C%20or,second%20set%20(the%20codomain).