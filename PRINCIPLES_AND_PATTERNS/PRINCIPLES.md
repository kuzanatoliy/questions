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


## Principles of Component Cohesion

<details>
  <summary>What is the Reuse/Release Equivalence Principle (REP)?</summary>

The granular of reuse is the granular of release.

REP states that the granule of reuse, a component, can be no smaller than the granule of release. Anything that we reuse must also be released and tracked. It is not realistic for a developer to simply write a class and then claim that it is reusable. Reusability comes only after a tracking system is in place and offers the guarantees of notification, safety, and support that the potential reusers will need. REP gives us our first hint at how to partition our design into components. Since reusability must be based on components, reusable components must contain reusable classes. So, at least some components should comprise reusable sets of classes.

</details>

<details>
  <summary>What is the Common Reuse Principle (CRP)?</summary>

The classes in a component are reused together. If you reuse one of the classes in a component, you reuse them all.

This principle helps us to decide which classes should be placed into a component. CRP states that classes that tend to be reused together belong in the same component. Classes are seldom reused in isolation. Generally, reusable classes collaborate with other classes that are part of the reusable abstraction. CRP states that these classes belong together in the same component. In such a component, we would expect to see classes that have lots of dependencies on each other. A simple example might be a container class and its associated iterators. These classes are reused together because they are tightly coupled. Thus, they ought to be in the same component.

</details>

<details>
  <summary>What is the Common Closure Principle (CCP)?</summary>

The classes in a component should be closed together against the same kinds of changes. A change that affects a component affects all the classes in that component and no other components.

This is the Single-Responsibility Principle (SRP) restated for components. Just as SRP says that a class should not contain multiple reasons to change, CCP says that a component should not have multiple reasons to change. In most applications, maintainability is more important that reusability. If the code in an application must change, you would prefer the changes to occur all in one component rather than being distributed through many components. If changes are focused into a single component, we need redeploy only the one changed component. Other components that don’t depend on the changed component do not need to be revalidated or redeployed.

</details>

## Principles of Component Coupling

<details>
  <summary>What is the Acyclic Dependencies Principle (ADP)?</summary>

Allow no cycles in the component dependency graph.

The dependency structure must always be monitored for cycles. When cycles occur, they must be broken somehow. Sometimes, this will mean creating a new component, making the dependency structure grow.

</details>

<details>
  <summary>What is the Stable-Dependency Principle (SDP)?</summary>

Depend in the direction of stability.

Designs cannot be completely static. Some volatility is necessary if the design is to be maintained. We accomplish this by conforming to CCP. Using this principle, we create components that are sensitive to certain kinds of changes. These components are designed to be volatile; we expect them to change. Any component that we expect to be volatile should not be depended on by a component that is difficult to change! Otherwise, the volatile component will also be difficult to change. It is the perversity of software that a module that you have designed to be easy to change can be made difficult to change by someone else simply hanging a dependency upon it. Not a line of source code in your module need change, and yet your module will suddenly be difficult to change. By conforming to SDP, we ensure that modules that are intended to be easy to change are not depended on by modules that are more difficult to change than they are.


</details>

## Don’t Ask Principle

<details>
  <summary>What is the Tell, Don’t Ask Principle?</summary>

The Tell, Don't Ask Principle relies on a basic object-oriented foundation: to delegate an action to an object instead of asking an object for data.

</details>

## Law of Demeter

<details>
  <summary>What is Law of Demeter?</summary>

The Law of Demeter (LoD), also known as the Principle of Least Knowledge, is a set of object-oriented programming rules that puts restrictions on interactions between program modules.

The LoD helps you avoid a major problem that can arise when you try to create a chaining method: a knot of dependencies. When you have a knot of dependencies, it means that a change in one object in the code will force you to verify/recompile/redeploy the module with the object and all other modules that depend on it.

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
