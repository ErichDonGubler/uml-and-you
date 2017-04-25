# CS 3450: UML and You 
## A quick explanation of how to write UML consistently and expressively <!-- class: fragment -->

---

## UML

* It's short for "Unified Modeling Language"
* Goal: make sure we can all speak the same language in OOP design, independent of programming language.
* It originally came from Rational Labs employees who organized "UML Partners", who worked to develop standards for communicating the structure of and interaction between objects in OOP.

---

## UML

Note how we phrased that: "communicating the structure of and interaction between objects". In this class, we'll use three diagrams related to these two things:
* Structure
  * Class diagrams: describes objects **statically**
  * Object diagrams: describes objects at **runtime**, and how an object's members may look over the course of its lifetime
* Interaction
  * Sequence diagrams: describes ***execution flow*** by *showing method calls on the stack*

---

## UML

* Structure
    * Class diagrams
    * Object diagrams
* Interaction
    * Sequence diagrams

There are others, but we won't go into them. Many needs can be met with just these three, especially the class and sequence diagrams.

---

# Class diagrams

---

## Components in a Class Diagram

Class diagrams are used to describe objects **statically**.
* Note that we're not assuming anything about what will actually happen in the program -- we're just noting everything that the object *has* or *could have*.

The bread and butter of class diagrams are our object descriptions, which are usually one of:
* An **interface**
* A **class**

---

## Components in a Class Diagram

The bread and butter of class diagrams are our object descriptions, which are usually one of:
* An **interface**
* A **class**

They're usually represented by a box with a title and some text:

<img src="GenericObjectDescription.dot.png" alt="">

---

## Interfaces

`Interfaces` are the heart of object-oriented design. Most of the time, it's ideal to design objects in such a way that all we need to know is that they expose certain methods.

* Methods correspond to behaviors we expect each object to have -- the object is responsible for knowing what to do with the method call.
* Object may or may not use internal state (AKA "members") to implement the functionality of their interfaces.
    * We don't care, though -- we just want to know that we can expect them to let us use the methods we design, and that's it.

---

## Interfaces

<img src="./Interface.dot.png" alt="">

---

## Classes

Classes 

<img src="./SomeClass.dot.png" alt="">

---

## Interfaces vs. Classes

<div style="width: 100%; display: flex; align-items: center; justify-content: center;">
<img src="./SomeClass.dot.png" alt="">
<div style="width: 100px"></div>
<img src="./SomeClass.dot.png" alt="">
</div>

---

