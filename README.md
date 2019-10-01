# Little dudes notation (v. 0.1.0)

![](https://i.imgur.com/HwyVhHw.png)

This notation reflects particular traits of your object-oriented code as little dudes with 

## Motivation

- to help developers quickly grasp essence of pieces of code
- to provide a compact way to reflect code complexity
- to visualize "bigger picture" in real projects
- to see how things change in dynamics 

## Foundation

1. Dudes - objects
2. Arms (or any other limbs) - methods
3. Fingers - parameters
4. "@"-symbols in the brain - instance variables
5. "Internal" hands - private methods
6. Swallen hands - too much conditional logic
7. Legs - same as hands (can be used to reflect "getter" methods)
8. Spawning platforms - classes

## Examples

```ruby
class Book
  attr_reader :title, :author
  def initialize(title, author)
    @title  = title
    @author = author
  end
end
```

![](https://i.imgur.com/Elqxq9s.png)

## Usage

1. [Example #1](https://github.com/inem/little-dudes-notation/blob/master/deconstruct-sandi-metz-talk.md)

## Learn More

Presentation "[Solving Architectural Problems with OOP in Pictures](https://speakerdeck.com/inem/solving-architectural-problems-with-oop-in-pictures)" 

## Flexibility

You don't have to visualize every single aspect of your class. For example, if for your task instance variables or private methods are not important, you simply don't draw them.

The same goes for classes/objects you want to reflect. For example, when you work on a feature or refactor a part of your code, you might be interested to visualize only a subset of classes.

## Extensibility

1. You can use colors to identify classes from different layers of abstractions, or classes of specific namespace.

2. Code coverage, code performance (Big-O notation), churn rate, vulnerabilities, any code complexity metrics can be easily reflected on bodies of the dudes.
