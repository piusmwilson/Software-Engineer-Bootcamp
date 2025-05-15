# Software Design Principles

Software design principles guide developers in creating efficient, scalable, and maintainable software. Here's a list of some of the most essential software design principles:

[1.] **𝗞𝗲𝗲𝗽 𝗜𝘁 𝗦𝗶𝗺𝗽𝗹𝗲, 𝗦𝘁𝘂𝗽𝗶𝗱 (KISS):**

 Keeping code as simple and clear as possible. Simple code is easier to understand and maintain and less prone to errors.

- Therefore designing and developing software products should be as simple as possible through using clear and concise code, avoiding unnecessary complexity, and focusing on the essential features.

[2.] **𝗗𝗼𝗻'𝘁 𝗥𝗲𝗽𝗲𝗮𝘁 𝗬𝗼𝘂𝗿𝘀𝗲𝗹𝗳 (DRY):**

  Avoid duplication in code and try to reuse code instead of copying it where and if necessary, to avoid inconsistencies and bugs in Software.
  
Therefore:

- Code should not be duplicated.
- Use functions and classes to encapsulate common code.
- Use variables and constants to store values that are used in multiple places.

[3.] **𝗬𝗔𝗚𝗡𝗜 (You Aren't Gonna Need It):**

 Avoid adding unnecessary complexity by adding functionality only when needed. You don't need to add extra features to software that you don't need, thereby keeping the software simple and maintainable.

[4.] **SOLID**

𝗦𝗢𝗟𝗜𝗗 𝗽𝗿𝗶𝗻𝗰𝗶𝗽𝗹𝗲𝘀 are a key set of principles in object-oriented programming that steers developers towards creating maintainable, scalable, and robust software architectures. They were introduced by Robert C. Martin (Uncle Bob), although they were influenced by earlier work from others.

- **Single Responsibility Principle (𝗦𝗥𝗣):-** A class should have a single focus or only one responsibility, making the system modular and easier to manage. This means a class should have only one reason to change. When a class encapsulates a single responsibility, changes in specifications will likely affect fewer components, making maintenance less complex. It also reduces coupling between different elements.

For example, we can have a 𝚄𝚜𝚎𝚛𝙼𝚊𝚗𝚊𝚐𝚎𝚛 class to handle different user-related operations, such as authentication, DB interaction, e-mail notifications, etc. If we change, e.g., the e-mail notification logic, it could affect other areas like user authentication. Such classes are sometimes called God classes.

- **Open/Closed Principle (𝗢𝗖𝗣):-** Software entities (classes, methods, etc.) should be open for extension but closed for modification, which promotes stability and extensibility. This means you can add a new functionality to a class without changing its existing code.

- **Liskov Substitution Principle (𝗟𝗦𝗣):-** Objects of a derived class (_subtypes_) should be substitutable for objects of the base class(_their base types_), ensuring seamless integration and robustness. This means if a class inherits some other class, you should be able to use it in the same way as the base class.

- **Interface Segregation Principle (𝗜𝗦𝗣):-** Clients should not be forced to depend on methods that they do not use or a class should not be forced to implement interfaces it does not use. This means creating specific interfaces for each class rather than having one large, all-encompassing one.

- **Dependency Inversion Principle (𝗗𝗜𝗣):-** Dependencies should be injected into a class rather than being hard-coded. High-level modules should not depend on low-level ones; both should depend on abstractions, encouraging a decoupled architecture. Also, abstractions should not rely on details; details should depend on abstractions.

[5.] **Principle of Least Astonishment/Surprise**

Suggests that a solution or approach would not surprise a reasonably knowledgeable person in the subject area when encountered for the first time.

Therefore:

- Design software in a way that is consistent with the user's expectations.
- Use familiar terminology and conventions, and provide clear and concise instructions.
- Use proper and concise error messages.

[6.] **Principle of Modularity**

- Design software as a collection of independent modules.
- This can help to make the software easier to understand, maintain, and test.

[7.] **Principle of Abstraction**

- Design software by hiding the implementation details from the user.
- This can help to make the software easier to understand and use.

[8.] **Principle of Encapsulation**

- Software should be designed to hide the internal state of an object from the outside world.
- This can help to make the software more robust and maintainable.

[9.] **𝗖𝗼𝗺𝗽𝗼𝘀𝗶𝘁𝗶𝗼𝗻 𝗢𝘃𝗲𝗿 𝗜𝗻𝗵𝗲𝗿𝗶𝘁𝗮𝗻𝗰𝗲**

Favoring object composition over class inheritance, as it's more flexible and helps to avoid problems associated with larger inheritance hierarchies.

[10.] **Principle of Least Knowledge (𝗟𝗮𝘄 𝗼𝗳 𝗗𝗲𝗺𝗲𝘁𝗲𝗿 (LoD))**

An object should only communicate with its immediate friends and not know other objects' inner workings. Software should be designed to minimize the amount of knowledge that a module needs about other modules which can help to make the software more modular and flexible.

[11.] **Principle of Low Coupling & High Cohesion**

- Coupling refers to the degree to which the elements of a module depend on each other.
- A module with low coupling has few dependencies and its elements do not depend on each other too much.
- Cohesion refers to the degree to which the elements of a module belong together.
- A module with high cohesion has a single, well-defined purpose and all of its elements are related to that purpose.