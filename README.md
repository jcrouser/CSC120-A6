# A6: Unit Testing
The goal of this assignment is to reinforce the importance of unit testing in Java using `JUnit`. You will design and implement a suite of unit tests for the train simulation we wrote A4: Chugging Along. Your A4 solution consisted of the following classes:

`Car`: Represents a train car.
`Engine`: Represents the train’s engine.
`Passenger`: Represents passengers who board and leave the train.
`Train`: Represents an entire train with one or more cars.

In this assignment, you will write at least **10 unit tests** that verify the functionality and correctness of each of these classes.

## Step 1: Getting Started
 - Fork the the repository for CSC120-A6, and clone it to your local machine.
 - Add your `Car.java`, `Engine.java`, `Passenger.java`, and `Train.java` to your forked repository and commit your changes.
 - Analyze the functionality of the classes contained in those files.
 - Enable Java tests using the `jUnit` testing framework.

## Step 2: Writing Unit Tests
Write your `jUnit` tests inside `TrainTest.java`, using **assertions** to validate expected outputs. Below you'll find a list of key methods in each class that should be tested:

### `Engine` Class (2 tests)
- Verify that the `Engine` constructor initializes correctly with the given `FuelType` and fuel level.
- Test the `go()` method to ensure that fuel consumption reduces the fuel level correctly.

### `Car` Class (2 tests)
- Ensure that adding a `Passenger` increases the passenger count.
- Check that removing a `Passenger` decreases the count and doesn't go negative.

### `Passenger` Class (2 tests)
- Test that a `Passenger` can successfully board a `Car`.
- Ensure that a `Passenger` cannot board a full `Car`.
  
### Train Class (4 tests)
- Verify that a `Train` initializes correctly with a given number of `Car`s.
- Ensure the `Train`’s total `Passenger` count updates as `Passenger`s board and leave.
- Check that the `getCar(int i)` method returns the expected `Car`.
- Test the `printManifest()` method to ensure it iterates through the `Train`s `Car`s correctly.

These are only a starting point; you are welcome to write additional tests if you would like.

## What to Submit
As before, all the files necessary for this assignment are contained within this repository. When you submit, please remember to include:

- all files necessary to compile your program
- `reflection.md` containing your reflections and notes
- `rubric.md` where you document which elements of the assignment you have attempted and/or completed
