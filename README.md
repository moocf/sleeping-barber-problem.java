There is a barber sleeping in his shop. When a customer comes, he checks if the barber is sleeping and wakes him up. If there are no other customers in the waiting room, the barber cuts his hair. Else the customer takes a set in the waiting room. But if there are no seats, he leaves. Once a barber finishes cutting hair, he checks if there are any customers in the waiting room. If not, he goes back to sleep again. The idea is the barber works only when a customer arrives, and sleeps otherwise.


The barber is providing 24x7 service:

1. sleeps until a customer wakes him up
2. he picks first customer in room (b.release)
3. one seat is freed up (seats++)
4. cuts customer's hair (sleep 1s)
5. ... goes back to sleep

Each customer requires a haircut:

1. occupies a seat, if available
2. wakes up the barber (c.release)
3. waits for barber to indicate his turn
4. ... his hair is cut.


See [Main.java] for code, and [repl.it] for output.

[Main.java]: https://repl.it/@wolfram77/sleeping-barber-problem#Main.java
[repl.it]: https://sleeping-barber-problem.wolfram77.repl.run


### references

- [Sleeping Barber Problem : Classical Problem of Process Synchronization :: HowTo](https://www.youtube.com/watch?v=OvJFpsN5czg)
