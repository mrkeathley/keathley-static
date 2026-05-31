---
title: "Hello, World! A Children's Bible Lesson"
date: 2023-06-16T16:52:00-05:00
draft: false
tags:
  - theology
  - coding
  - philosophy
---
> I am not really happy with this at the moment. But it's an interesting idea as a children's bible lesson for a coder's camp. It might be worth running with someday.

The act of creation is the first act of God revealed in Scripture. We see this in the opening words of the Bible: “In the beginning God created the heavens and the earth” (Genesis 1:1). This creation brings about all things that are not God in a single amazing moment—not from preexisting materials, but from nothing. The traditional Latin phrase for this is *ex nihilo*, meaning “from nothing.”

This creative act is described in two broad categories: the heavens and the earth. The heavens include everything above: the stellar and cosmic phenomena of the universe. They may also include spiritual entities and realities beyond the visible world. The earth includes the matter that makes up our home. Together, the heavens and the earth form the logical beginning of the cosmos.

As humans, we are blessed to join with God in small acts of creation. Unlike that first moment, we are not able to create from nothing. Instead, we reorganize the components we have been given in new ways. In Genesis, we see that God creates by speaking: “And God said, ‘Let there be light,’ and there was light” (Genesis 1:3). In computer programming, we are able to imitate this behavior, though only in a limited and creaturely way. We speak ideas and purposes into a computer and see it spring into action. To do this, we use a vocabulary and a set of grammatical rules for instructing a computer to perform tasks. This is called a programming language.

Traditionally, the first program written by novice computer scientists is called “Hello, World!” The goal is to lay enough of a foundation in the code to have the computer return the words “Hello World” to the operator. Depending on the programming language and tools used, this can be as simple as a single line or much more complicated. In this study, we will give instructions to the computer using the Python programming language, which is designed to be readable, easy to learn, and relatively unambiguous.

Let’s take a look at a “Hello World” program written in Python:

```python
print('Hello World')
```

Easy!

Following God’s creative decree at the beginning of Genesis, we see a series of creative acts that produce distinction, order, and hierarchy where none had existed before. God creates light, water, sky, and land with purpose and intentionality. He also produces vegetation and living creatures according to their kinds.

This pattern of category and structure is something we still recognize in the field of biology today. For example, we have the broad category of mammals. Under mammals, there are more specific categories, such as primates and felines. Under those, there are even more specific categories, such as humans, chimpanzees, lions, and domestic cats. Each subsequent category shares certain traits with the category above it while also adding unique traits of its own.

This hierarchy is not merely an idea that describes how things are arranged in the biological world. It is a fundamental principle of structure that applies across many fields, including computer science. This principle is at the heart of what we call Object-Oriented Programming, often abbreviated as OOP.

In OOP, we define a “class” as a blueprint for creating “objects.” A class may define attributes, which are characteristics, and methods, which are behaviors. Objects created from a class receive those attributes and methods. Classes can also inherit from other classes, allowing a more specific class to receive traits from a more general class while adding traits of its own.

Take Python, for instance. Let’s model our example of mammals, primates, and humans in Python code. You are not expected to understand all of this at first, but we will walk through it step by step.

```python
class Mammal:
    def __init__(self):
        self.has_hair = True
        self.is_warm_blooded = True

    def display_traits(self):
        return f"Has hair: {self.has_hair}, Is warm-blooded: {self.is_warm_blooded}"

class Primate(Mammal):
    def __init__(self):
        super().__init__()
        self.has_opposable_thumbs = True

    def display_traits(self):
        parent_traits = super().display_traits()
        return f"{parent_traits}, Has opposable thumbs: {self.has_opposable_thumbs}"

class Human(Primate):
    def __init__(self):
        super().__init__()
        self.can_speak = True

    def display_traits(self):
        parent_traits = super().display_traits()
        return f"{parent_traits}, Can speak: {self.can_speak}"

john = Human()
print(john.display_traits())
# Returns: "Has hair: True, Is warm-blooded: True, Has opposable thumbs: True, Can speak: True"
```

In this example, the `Human` class is a subclass of `Primate`, which is itself a subclass of `Mammal`. Each subclass inherits the characteristics of the superclass and can also add new characteristics.

Boolean logic is another fundamental concept in computer science and mathematics. It is named after George Boole, a nineteenth-century British mathematician and logician. Boolean logic includes the basic logical operations AND, OR, and NOT. These operations are building blocks for more complex logical expressions.

In a theistic worldview, these fundamental principles of logic can be understood as reflections of God’s nature. If God is perfectly logical and consistent, then the logic we see in the universe, including Boolean logic, reflects something about the divine nature. Logic and order exist because they are grounded in God himself and are woven into the fabric of creation.

As an example in Python, consider this simple piece of code using Boolean logic:

```python
a = True
b = False

# AND operation
print(a and b)  # returns False

# OR operation
print(a or b)   # returns True

# NOT operation
print(not a)    # returns False
```

This script represents the basic principles of Boolean logic. The AND operation returns `True` only if both operands are `True`. The OR operation returns `True` if at least one of the operands is `True`. The NOT operation inverts the value of the operand.

Similarly, mathematics, including number theory and geometry, can be seen as an expression of the divine order in the universe. The patterns, symmetries, and relationships that we find in mathematics can be understood as reflections of God’s mind—an expression of the way God has ordered reality. The mathematical truths we discover were not created by us. Rather, we discover them as we explore the ordered structure of the universe.

An example of this can be seen in the Fibonacci sequence. Here is one way to generate a Fibonacci sequence in Python:

```python
def fibonacci(n):
    if n <= 0:
        return "Input should be a positive integer."
    elif n == 1:
        return [0]
    elif n == 2:
        return [0, 1]
    else:
        fib_sequence = [0, 1]
        for i in range(2, n):
            next_value = fib_sequence[i - 1] + fib_sequence[i - 2]
            fib_sequence.append(next_value)
        return fib_sequence

print(fibonacci(10))  # returns [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```