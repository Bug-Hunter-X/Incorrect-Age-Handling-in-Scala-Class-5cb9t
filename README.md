# Incorrect Age Handling in Scala Class

This repository demonstrates a common error in Scala class design related to improper handling of invalid input in setter methods.

## Bug Description
The `MyClass` class uses a setter method (`age_=`) to update the age of a person. However, the setter method throws an `IllegalArgumentException` if a negative age is provided which is generally considered bad practice.

## Bug Solution
The improved solution handles the invalid input gracefully, either by ignoring the update, using a default value, or returning a result that indicates failure.

## How to Run
1.  Clone this repository.
2.  Compile and run `MyClass.scala` using a Scala compiler (e.g., `scalac MyClass.scala` and then `scala Main`).