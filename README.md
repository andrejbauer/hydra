# The hydra game

The Hydra is a rooted tree. The object of the game is to chop off all its heads (the blue
disks). At step `n`, when you cut a head, the Hydra will grow `n` new copies of the tree
growing from the neck at which the head was cut.

A theorem by Paris and Kirby [1] states that *you always win*, no matter how you chop the
heads, but it takes a rather long time to chop down a hydra. Paris and Kirby also showed
that Peano arithmetic does not prove that hydra always loses.

## About the program

The Hydra game is implemented in Java and is packaged as an Eclipse project. I have
released the source code into the public domain. Please send me any enhancements you
implement on top of my code.

## How to run the program

You may run the main program `HydraWindow` from Eclipse or directly from command
line with (you need to change to the `src` directory first)

    CLASSPATH=bin java hydra.HydraWindow

Alternatively, you can download the JAR file and run it with

    java -jar hydra.jar
  
The game can be embedded into a web page as a Java applet, for which you should
use `hydra.JavaApplet`, see the file [`hydraApplet.html`](hydraApplet.html).

### References

[1] Laurie Kirby and Jeff Paris: [Accessible Independence Results for Peano Arithmetic](http://faculty.baruch.cuny.edu/lkirby/accessible_independence_results.pdf). Bull. London Math. Soc. 1982; 14: 285-293.

