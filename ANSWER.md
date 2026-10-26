1. GitHub Repository Link

https://github.com/shanahjoyatienza-glitch/flutter_basics_lab

2. Activity 2 — Last Three build() Lines
Copy the actual last three lines from your Debug Console here.


build() called: 4 glasses
build() called: 5 glasses
build() called: 6 glasses
Note: These are examples. Replace them with the actual last three lines from your Debug Console.

3. Observations from the Experiments
Activity 2 — setState()
When I moved _glasses++ outside setState(), the counter did not update immediately because Flutter was not notified to rebuild the screen.

Activity 3 — Expanded
When I removed Expanded from a StatBox, the boxes became uneven in size and could overflow the screen. Expanded makes the boxes share the available space.

Activity 5 — ThemeData
I changed the button corner radius from 8 to 20. The buttons became more rounded and looked softer.

1. What is the difference between a StatelessWidget and a StatefulWidget? Give one example of each.

-A StatelessWidget does not change its own state, like ProfileCard in Activity 1. A StatefulWidget can change its appearance when the data changes, like WaterTrackerPage in Activity 2.

2. Why is a StatefulWidget written as two classes? What does each class do?

-The first class creates the widget, while the second class stores the changing data and updates the screen.

3. In Activity 2, what happened when you changed _glasses outside setState()? Why?

-The number on the screen did not update because Flutter was not told to refresh the screen.

4. When is build() called in Activity 2?

-It is called when the app first opens and when setState() updates the screen.

5. Explain the main axis and cross axis of a Row and a Column.

-In a Row, the main axis is horizontal and the cross axis is vertical. In a Column, the main axis is vertical and the cross axis is horizontal.

6. What happened when you removed Expanded from a StatBox? What does Expanded do?

-The boxes became uneven in size and could overflow the screen. Expanded makes the boxes share the available space.

7. Why do we use GridView.builder instead of a Column with many children?

-GridView.builder displays items in rows and columns and allows scrolling. A Column only arranges items vertically.

8. How do Stack and Positioned create the Best seller badge in Activity 4?

-Stack allows widgets to overlap, while Positioned places the Best seller badge in a specific spot on the card.

9. What is the difference between ThemeData and a style on one widget? Give one example of each.

-ThemeData changes the general appearance of the app, like the button corner radius. A widget style changes only one widget, like making the “My skills” text bold.

10. When you flip the dark-mode switch, which widget holds the state, and how does the change reach MaterialApp?

-ThemeDemoAppState holds the _isDark variable. When I flip the switch, setState() updates the value, and MaterialApp changes to dark or light mode.