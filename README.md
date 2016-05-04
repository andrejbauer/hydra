# The hydra game

The Hydra is a rooted tree. The object of the game is to chop off all its heads (the blue
disks). At step `n`, when you cut a head, the Hydra will grow `n` new copies of the tree
growing from the neck at which the head was cut.

A theorem by Paris and Kirby [1] states that *you always win*, no matter how you chop the
heads, but it takes a rather long time to chop down a hydra. Paris and Kirby also showed
that Peano arithmetic does not prove that hydra always loses.

The Hydra game is implemented in Java. I have released the source code into the public
domain. Please send me any enhancements you implement on top of my code.

You may run the program in several ways:

1. Run the game as an [applet in your browser](http://math.andrej.com/wp-content/uploads/2008/02/Hydra/hydraApplet.html) (you may have to convince the brower that this is not a secuirty risk).

2. [Download the JAR file `hydra.jar`](http://math.andrej.com/wp-content/uploads/2008/02/hydra.jar) and run it on your computer by double-clicking on it or from the command line

       java -jar hydra.jar

3. Run `HydraWindow` from your IDE if you know what that means

2. Change to the repository directory, compile the program

       javac -d bin -sourcepath src src/hydra/HydraWindow.java       

   and run it with

       CLASSPATH=bin java hydra.HydraWindow
  

#### References

[1] Laurie Kirby and Jeff Paris: [Accessible Independence Results for Peano Arithmetic](http://faculty.baruch.cuny.edu/lkirby/accessible_independence_results.pdf). Bull. London Math. Soc. 1982; 14: 285-293.

