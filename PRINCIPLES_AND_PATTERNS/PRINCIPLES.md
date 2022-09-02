# Principles

## SOLID

<details>
  <summary>What is SOLID?</summary>

- The single responsibility principle - each class should have only one reason to change. Everything within a class should do one thing, so there is only one reason for the class to change. If you are thinking about the responsibilities of a class and adding “and” to describe them, it means that the class may have several reasons to change in the future when you need to scale or update your application. Creating classes that focus on one purpose each, however, will make your code easier to understand and maintain.

- The open-closed principle - each entity should be open for expansion and be closed for modification.
  Open for extension means that the behavior of the module can be extended. As the requirements of the application change, we are able to extend the module with new behaviors that satisfy those changes. In other words, we are able to change what the module does.”
  Closed for modification means that the extending the behavior of a module does not result in changes to the source or binary code of the module. The binary executable version of the module, whether in a linkable library, a DLL, or a Java .jar, remains untouched.

- The Liskov substitution principle - any subclass should supplement the parent class but not change it. It extends the second SOLID principle—the OCP—by focusing on the behavior of a supertype—which is a base or parent class—and its subtypes—which are derived or child classes.

- The interface segregation principle - a few separate interfaces are better than one combined interface.
  These benefits demonstrate why the ISP helps you develop interfaces that are effectively designed and minimize the impact of modifications.
  While you can add a new method to an existing interface, if the new method implements a different responsibility, it’s best to separate it into a new interface. Implementing new methods without considering potential effects can lead to unintended and undesirable results, so it’s best to adhere to this principle from the start.

- The dependency inversion principle - dependencies should be only on abstractions.
  Applying the DIP prevents changes to low-level modules from impacting and forcing changes to high-level modules. It also guarantees that abstractions do not depend on details since these dependencies can also force unnecessary code changes.

</details>

## Don’t Ask Principle

<details>
  <summary>What is the Tell, Don’t Ask Principle?</summary>

The Tell, Don't Ask Principle relies on a basic object-oriented foundation: to delegate an action to an object instead of asking an object for data.

</details>

## KISS

<details>
  <summary>What is KISS?</summary>

KISS or keep it simple stupid is one of the design principles. KISS says that the many systems will work better if they are simple. So, simplicity should be one of the main targets in the design sphere.

</details>

## DRY

<details>
  <summary>What is DRY?</summary>

DRY or don’t repeat yourself is one of the design principles. DRY says that not need to repeat different information or functionality. Each part of knowledge should have only one view into system scope.

</details>

## YAGNI

<details>
  <summary>What is YAGNI?</summary>

YAGNI or you aren’t gonna need it is one of the design principles. YAGNI says that the programmer should not implement functionality if it is not necessary. There are a few reasons. Firstly, a customer does not have to pay for something that is not needed for him. Secondary, additional functionality could increase the development difficulty of other features.

</details>
