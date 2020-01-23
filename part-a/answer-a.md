## Part a

### Describe what the code in `z3-test.py` is doing in a paragraph or two.

 The code first defines Boolean objects a,b and Integer objects x,y, then it creates a logical statement f, consisting of several conditions that we want a,b,x,y to satisfy. It then instantiates a solver, prints the statement f, and uses the solver to check if we can satisfy the condition through some values of a,b,x,y, printing the result as either "sat" or "unsat". If f is satisfied, it then prints one instance of a,b,x,y that satisfies it. For the second part, it adds another condition to the solver and repeats the same process. 

 The output shows that the statement And(Not(a), b, x > 0, x < 100, x < y) can be satisfied with [x = 99, y = 100, b = True, a = False], but the statement [And(Not(a), b, x > 0, x < 100, x < y), y < 1] cannot be satisfied. 