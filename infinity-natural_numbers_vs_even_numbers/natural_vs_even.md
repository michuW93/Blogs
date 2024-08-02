# Natural numbers vs Even numbers

I would like to start with question - is there as many natural numbers as even numbers?<br>
Intuition says no but let's check it.

What does it even mean that sets have the same size? Well, they have the same number of elements, right?<br>
Example:<br>
set A = {1,2,3} <br>
set B = {5,6,8} <br>

these are the same size. Both set A and set B have 3 elements. <br><br>


That was easy because we could count number of elements. It's worse when we would like to count number of elements in infinite set.<br>
You can think of the biggest number you can imagine and you can always add 1 to it. So it's impossible to count them in a way we did in first example.<br>

There is another option, we can try to pair elements from both sets. If we go back to previous example we can see that all elements from set A have a pair in set B.<br>
Pair for 1 from A will be 5 from B, pair for 2 from A will be 6 from B and pair for 3 from A will be 8 from B.<br>
Okay, we again showed that sets size are the same even though we didn't count them. <br>
Moreover, we created **bijection** between two sets. Bijection seems like something really tricky and hard in math, but it's basically function one to one.<br>
If you can find for every element from A corresponding element from B then it's bijection, if you can't - it's not.<br><br>


Let's switch to more interesting problem if we already have idea how to deal with it - are there as many natural numbers as even numbers?<br>
Again we have two sets (N natural, E even):<br>
N = {0, 1, 2, 3, 4, ...}<br>
E = {0, 2, 4, 6, 8, ...}<br>

If we were to rely on our intuition, we might assume that set N is larger because it contains the same numbers as even numbers set, plus an additional elements (e.g. 3 or 5).<br>
Yes but still there is no option to count it so let's try to use our second idea - let's pair them or find bijection as it's sound cooler.<br>
For 0 from N we have 0 from E<br>
for 1 from N we have 2 from E<br>
for 2 from N we have 4 from E<br>
...<br>
for n from N we have 2N from E<br>

we just showed that every element from N has corresponding element in E! All elements have a pair so size of N and E must have the same size! <br>

Conclusion: **We have as many natural numbers as even numbers!**



Additional note - if you are interested how to check if number is even in best way see my comment: [https://www.youtube.com/watch?v=OCieTLLrazI&ab_channel=TVPSport](https://stackoverflow.com/a/51998794/4952262)<br>
https://math.stackexchange.com/questions/341605/as-many-even-numbers-as-natural-numbers<br>
https://en.wikipedia.org/wiki/Bijection#:~:text=A%20bijection%2C%20bijective%20function%2C%20or,second%20set%20(the%20codomain).<br>
