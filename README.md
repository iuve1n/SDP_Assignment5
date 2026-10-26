# Calculator with Strategy Pattern

This Java project demonstrates the Strategy pattern with a calculator. The calculator can use addition, subtraction, or multiplication, and the Client can change the selected operation while the program runs.

## Build and run

Use JDK 17 or later. From the project folder, run:

```sh
mkdir -p out
javac -d out src/strategy/*.java
java -cp out strategy.Client
```

## Add another operation

Create a class that implements `CalculationStrategy` and defines its `calculate` method. In the Client, pass an instance to the `Calculator` constructor or call `setStrategy` to switch to it. The `Calculator` works with the interface, so adding an operation does not require changing its calculation method.
