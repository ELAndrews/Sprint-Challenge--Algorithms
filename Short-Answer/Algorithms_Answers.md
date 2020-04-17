#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n) => This is an example of linear time complexity. This is because the code has to be executed step by step, with each incrementation, until it reaches it fall out of `a < n * n * n`.


b) O(log(2)) => This is an example of logarithmic time complexity. Within the first for loop the variable j is defined, followed by a while loop. j is incremented by *= 2 resulting in j increasing exponentially.


c) O(n) => This is another example of linear time complexity. This is because the recursive function is called step by step, with each decrement of bunnies. This will therefore fun through each bunnie in the list before the fall out of `bunnies == 0`. 

## Exercise II

pre answer notes:
- number of floors => n => search of floor f (drop egg => break=lower, fine=higher)=> return floor f
- binary tree:               n
                            /  \
                    a=[:n/2]   b=[n/2:]
                     /  \         /   \
                [:a/2] [a/2:]  [:b/2] [b/2:]
- use recursive function until floor f found



pseudocode:

function find_f(takes range of floors):
    if range of floors is 1:
        return number of floors
    
    at range of floors / 2
        if egg fine:
            find_f(passing: range of floors / 2 as lowest, range of floors max)
        if egg breaks:
            find_f(passing: range of floors min, range of floors / 2 as highest )


runtime:

O(log(n))