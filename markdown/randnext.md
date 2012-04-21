
#randnext

##Syntax
**randnext** ( **var** *v* : **real**, *seq* : 1 .. 10 )

##Description
The **randnext** procedure is used when you need several sequences of pseudo-random numbers, and you need to be able to exactly repeat these sequences for a number of simulations. The **randnext** procedure is the same as **rand**, except *seq* specifies one of ten independent and repeatable sequences of pseudo-random real numbers.
The **randseed** procedure is used to start one of these sequences at a particular point.

##See also
**[randseed.html](randseed)**, **[randint.html](randint)**, **[rand.html](rand)** and **[](randnext)**.