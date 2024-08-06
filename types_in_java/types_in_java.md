# Types in java

Last weeks I was doing interviews on senior java developer role. I’m surprised by how many people are familiar with Java types only at a surface level.<br>

##Integer - everyone uses, not a lot of knows it deeper
During interviews, I was asking people: you have java class with field age. What type would you use for this?
Nearly all people said Integer and it's correct. So I asked what is the max value of Integer and how many bits it has in Java and here I heard maybe two good answers.
Of course, I am not expecting answer 2147483647 but I would like to hear about 2 billions. Also I was surprised that nearly noone knows that Integer in Java has 32 bits.
Okay, but is it even important? Well, for age you don't need to know max value of Integer but what if you would like to store value of all person shares?
Let's say that he has 1000 shares of Lindt which is now around 10 000 CHF. Will it be enough? What if we would like to change currency to polish zloty or turkish lira?
That's why it's important. In my opinion all Java developers should know that to check max value should use `Integer.MAX_VALUE`, that it's slightly over 2 billions
and that <b>Integer has 32 bits</b>. Actually max value of Integer is 2^32-1? Why? Because there are 2^32 possibilities of all values but first bit is sign (- or +)[1].
If you know that you need something bigger than Integer then go for Long or even BigInteger.

##Float vs Double
The next question about types is differences between Double and Float. Usually everyone knows that Double has wider range but again in case of 
max values and bits it's the same as in previous chapter. <b>Double has 64 bits, Float has 32 bits</b>.

##Problem with floating point
I also like to ask about problem with floating point. What is the problem?<br>
From System.out.println(2.00-1.10) I would expect result 0.9, however for some reason I receive 0.899999. Why is that and how to fix it?
This one is a bit more complicated. 

[1]https://stackoverflow.com/questions/5771520/why-is-the-maximum-value-of-an-unsigned-n-bit-integer-2%e2%81%bf-1-and-not-2%e2%81%bf