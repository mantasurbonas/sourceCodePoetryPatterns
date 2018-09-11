# Source Code Poetry Patterns

## Rhymed elements of source code


Over the years, the elite Source Code Poetry competition has attracted multiple talented artwork in a field of computer-compilable source code poetry. Building on that experience, we can now firmly establish that certain elements of source code can be safely applied in multiple real-life applications, bringing the production code base to another level of sophistication.



## Pattern #1. Main Method

### Intent
Make your main method less boring by making boilerplate code rhyme.

### Motivation / Problem Description

Most of Java applications need a boring entry point. This "entry point" is a static method that adheres to certain specific Java language conventions: i.e. it must be named "main", it has to accept certain type of parameters, return nothing  etc.

```java
public class Main{
 
   public static void main (String args[]){
      // your initialization code here
   }
 
}
```
Figure 1. A typical entry point of a typical Java application.

The Java language syntax enforces certain keywords that significantly restrain freedom of artistic expression.
However you yourself don't have to be that boring and restricted. 

### Implementation / Solution
The application's entry point can be written in a human-readable two-liner rhyme:
```java
	public static void main ( String [] 
	is) { where ( new Life(), Shall::begin ); }
	
	static class Life{
		static{
			// place your initialization code here
		}
	}
```
Figure 2. A main method that rhymes.

This two-liner is an instant dramatic improvement over the “standard” non-poetic code.
Obviously, the code above does need some extra code (a so called "boilerplate code") to actually work. 
In case you have sufficient degree of freedom in your project, you should be able to create necessary classes elsewhere in your application structure - or use a SourceCodePoetry.jar lib as a project dependency.
However it happens that team members are occasionally not that receptive to a poetic code. You would need to place all the boilerplate code within the same class, which makes entry point class somewhat less laconic as illustrated in a code below:

```java
public class Main{
 
	public static void main ( String [] 
	is) { where ( new Life(), Shall::begin ); }
	
	static class Life{
		static{
			// place your initialization code here
		}
	}
 
	// boilerplate code down here.
	// could be moved to a separate library.
	// not really a sound poetry.
	
	static class Shall{
	static int   begin(
	Life starts, 
	Life smiles) 
	{ return 1000000; }}
 
	
	static Life 
	where ( Life begins, 
	Comparator <? extends Life> 
	and) { return begins; }
}
```
Figure 3. Self-contained main class, rhymed entry point, and the boilerplate code.

### Consequences
The first committer of such code receives instant attention from peer reviews. 
An immediate feedback from your team may vary, depending on the individual level of poetic maturity of your team members. Some less-enlightened personalities are known to be rather melodramatic about the obviously improved code interestingness quality. 
This type of reaction helps you better experience the emotional state of world’s greatest artists like Vincent van Gogh or Paul Gauguin, who all faced severe adversity from their peers for being ahead of their time.
In either occasion, the emotional equilibrium of the project team gets an additional charge. 

From a scientific perspective, it has been empirically proven that Java programmers can be easily trained into a semi-automatic reaction, where a commonly used phrase “public static void main string” triggers an immediate sub-conscious response with “… is where new life shall begin”. 
