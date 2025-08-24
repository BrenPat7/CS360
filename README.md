# CS360
Android App Development, Inventivy 

Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?

The app's main goal was to allow users to efficiently manage and track inventory. It was designed to address the user need for a simple, intuitive tool to monitor quantity, generate reports, and add or remove items from this database.

What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?

To ensure a user-centered UI, the app required three main screens: a unified login/registration screen, a data display screen with CRUD functionality, and a dedicated screen for managing SMS notifications. These designs were successful because they prioritized a clear visual hierarchy, provided consistent feedback, and gave the user control over their experience.

How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?

I coded the app using a bottom-up approach, building the core database and data-handling logic first, and then implementing the UI on top of it. This strategy, which included techniques like separation of concerns and iterative development, ensures a stable foundation and allows for faster debugging and future scaling.

How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?

I tested the app by using the Android Emulator to simulate the user experience on a virtual device. This process was crucial because it allowed me to identify and fix bugs in a controlled environment before the app could reach real users. Testing revealed a critical bug where the app crashed after a successful login because the database table for inventory items did not exist.

I had to innovate to overcome a challenge in the database implementation. When the app was trying to access the inventory table before it was created, I had to find a way to reinitialize the database to include the new table. The solution was to instruct the user to uninstall the app from the emulator. This forced the app to run the onCreate method in the LoginDatabase.java file again, which created the inventory_items table and fixed the crash.

The importance of this process is that it provides a way to ensure the app's code is functional and stable. It helped to identify a flaw in the database creation logic: the app was trying to access a table before it was created. This process is important because it can identify errors that are not visible during the coding process alone.

In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
My greatest success was in developing the SQLite database and its CRUD operations which provided a solid foundation for user authentication and inventory management, demonstrating a strong grasp of data persistence within a mobile app.
