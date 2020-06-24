# Concurrent Programming in Java  

These mini projects are programming assignments for Parallel Programming in Java offered by Rice University on Coursera, as a part of [Parallel, Concurrent, and Distributed Programming in Java Specialization](https://www.coursera.org/specializations/pcdp)

## Compiling  
### Compiling with Maven from Command Line

`$ mvn compile`

### Compiling with Maven using Intellij

Import project > select miniproject_ directory > Import project from external model, select Maven.

### Compiling Manually using Javac

You will need to add the following JARs to your classpath while building both the provided source and test files using javac

`$ javac -cp ./hamcrest-core-1.3.jar:./junit-4.12.jar:./pcdp-core-0.0.4-SNAPSHOT.jar:target/classes/:target/test-classes/ src/main/java/edu/coursera/parallel/Setup.java src/test/java/edu/coursera/concurrent/SetupTest.java`

## Testing

### Testing with Maven

`$ mvn test`

### Testing with Maven using Intellij

Navigate to View > Tool Windows > Maven. From the Maven Projects pane, expand the Lifecycle section and double-click "test" to automatically run the tests.

### Testing Manually from Command Line

`$ java -cp ./hamcrest-core-1.3.jar:./junit-4.12.jar:./pcdp-core-0.0.4-SNAPSHOT.jar:target/classes/:target/test-classes/ org.junit.runner.JUnitCore edu.coursera.concurrent.SetupTest`

## Contents

### miniproject_1

Locking and Synchronization

Writed code using the synchronized statement, Java locks, and Java read-write locks. Implemented a concurrent, *sorted* list data structure. 

### miniproject_2

Global and Object-Based Isolation

Implement a concurrent banking system that can accept transactions from many threads of execution at once. 

Used object-based isolation to protect bank accounts from concurrent accesses to ensure that all bank balances are correct, and enable more transactions per second than would be possible with global isolation.

### miniproject_3

Sieve of Eratosthenes Using Actor Parallelism

Implemented prime numbers generating algorithm using the Sieve of Eratosthenes.

Used actors to realize a parallel version of the Sieve of Eratosthenes.

### miniproject_4

Parallelization of Boruvka's Minimum Spanning Tree Algorithm

Explored the use of concurrent queues, threads, and unstructured locks, with calls to *tryLock()*.

Produced a concurrent and data race-free implementation of Boruvka's algorithm. 

Evaluated the performance on real datasets representing [the road networks of several United States regions](http://www.dis.uniroma1.it/challenge9/download.shtml).

## Author

Maiqi Ding
