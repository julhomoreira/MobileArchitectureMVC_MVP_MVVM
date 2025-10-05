# MobileArchitectureMVC_MVP_MVVM

 I created a single Android application that features a simple counter screen:
 · ATextView to display the current count (starting at 0).
 · AButton that, when pressed, increments the count by 1.
 · AResetButton that, when pressed, resets the count to 0

 -----------------------------------------------------------------------------

 	MVC, MVP, and MVVM

The goal of this study was to develop a basic counter application in three distinct architectures: MVC, MVP, and MVVM, within the same Android project. Although they all solve the same problem (incrementing and resetting a value), the way each pattern organizes responsibilities is quite different.
	In MVC, the Activity plays the role of the View, forwarding events to the Controller, which manages the Model and requests interface updates. The separation is clear, but the View still has some dependency on the Controller.
	In MVP, we implemented the Presenter, responsible for centralizing the interface logic. The View simply presents information and delegates actions, making it "simpler" and easier to test.
	Finally, in MVVM, the ViewModel provides observable states (using StateFlow), and the View simply monitors these changes. This promotes reactivity, state persistence across configuration changes, and scalability.
In comparison, MVC is simple and suitable for small applications, MVP improves testability and clarity, while MVVM is the most modern and recommended in the current Android ecosystem.
