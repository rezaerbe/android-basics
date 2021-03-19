# [Android Basics in Kotlin](https://developer.android.com/courses/android-basics-kotlin/course)

Welcome to Android Basics in Kotlin! In this course, you'll learn the basics of building Android apps with the Kotlin programming language. Along the way, you'll develop a collection of apps to start your journey as an Android developer.

## [Unit 1: Kotlin basics for Android](https://developer.android.com/courses/android-basics-kotlin/unit-1)

Take your first steps programming in Kotlin, add images and text to your Android apps, and learn how to use classes, objects, and conditionals to create an interactive app for your users.

### [Android Basics: Introduction to Kotlin](https://developer.android.com/courses/pathways/android-basics-kotlin-one)

Learn to code in Kotlin, a modern programming language that makes coding clear and accessible.

#### [Write your first program in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-first-kotlin-program)

In this codelab, you are going to write your first program in the Kotlin language using an interactive editor that you can run from your browser.

- https://developer.android.com/training/kotlinplayground is an interactive code editor on the web where you can practice writing Kotlin programs.
- All Kotlin programs need to have a `main()` function: `fun main() {}`
- Use the `println()` function to print a line of text.
- Place text you want to print between double quotes. For example `"Hello"`.
- Repeat the `println()` instruction to print multiple lines of text.
- Errors are marked red in the program. There is an error message in the output pane to help you figure out where the error is and what might be causing it.

#### [Create a birthday message in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-kotlin-birthday-message)

In this codelab you will create a short Kotlin program that prints a birthday message with a cake and a birthday banner.

- Use `${}` to surround variables and calculations in the text of print statements. For example: `${age}` where `age` is a variable.
- Create a variable using the `val` keyword and a name. Once set, this value cannot be changed. Assign a value to a variable using the equal sign. Examples of values are text and numbers.
- A `String` is text surrounded by quotes, such as `"Hello"`.
- An `Int` is a whole positive or negative number, such as 0, 23, or -1024.
- You can pass one or more arguments into a function for the function to use, for example: `fun printCakeBottom(age:Int, layers:Int) {}`
- Use a `repeat() {}` statement to repeat a set of instructions several times. For example: `repeat (23) { print("%") }` or `repeat (layers) { print("@@@@@@@@@@") }`
- A *loop* is an instruction to repeat instructions multiple times. A `repeat()` statement is an example of a loop.
- You can nest loops, that is, put loops within loops. For example, you can create a `repeat()` statement within a `repeat()` statement to print a symbol a number of times for a number of rows, like you did for the cake layers.

**Summary of using function arguments:** To use arguments with a function, you need to do three things:

- Add the argument and type to the function definition: `printBorder(border: String)`
- Use the argument inside the function: `println(border)`
- Supply the argument when you call the function: `printBorder(border)`

### [Android Basics: Create your first Android app](https://developer.android.com/courses/pathways/android-basics-kotlin-two)

Learn to create Android apps using Android Studio in this introductory pathway.

#### [Download and install Android Studio](https://developer.android.com/codelabs/basic-android-kotlin-training-install-android-studio)

In this codelab, you will learn how to download and install Android Studio, Google's Android development environment.

#### [Create and run your first Android app](https://developer.android.com/codelabs/basic-android-kotlin-training-first-template-project)

In this codelab, you'll create your first Android app (Happy Birthday) starting from a template for a basic app provided by Android Studio. You'll also explore what an Android project looks like, and learn how to use different windows in Android Studio.

- To create a new project, start Android Studio, click **+ Start a new Android Studio project**, name your project, choose a template, and fill in the details.
- To create an Android virtual device (an emulator) to run your app, choose **Tools > AVD Manager** and then use the [AVD Manager](http://developer.android.com/tools/devices/managing-avds.html) to select a hardware device and system image.
- To run your app on a virtual device, make sure you have created a device, select the device from the toolbar dropdown menu, and then run your app by clicking the **Run** icon ![choose Run > Run app or click the Run icon [ICON HERE] in the toolbar. [IMAGEINFO]: ic_run.png, Android Studio Run icon](https://developer.android.com/codelabs/basic-android-kotlin-training-first-template-project/img/609c3e4473493202.png) on the toolbar.
- To find your project files, in the **Project** window, select **Project Source Files** from the dropdown.

#### [Optional: Run your app on a mobile device](https://developer.android.com/codelabs/basic-android-kotlin-training-run-on-mobile-device)

### [Android Basics: Build a basic layout](https://developer.android.com/courses/pathways/android-basics-kotlin-three)

Learn how to add images and text to your Android apps.

#### [Create a Birthday Card app](https://developer.android.com/codelabs/basic-android-kotlin-training-birthday-card-app)

In this codelab, you will build a simple Android app that displays text. You will be able to position the text on the screen by understanding more about User Interface (UI) components in Android.

- The **Layout Editor** helps you create the UI for your Android app.
- Almost everything you see on the screen of your app is a `View`.
- A `TextView` is a UI element for displaying text in your app.
- A `ConstraintLayout` is a container for other UI elements.
- `Views` need to be constrained horizontally and vertically within a `ConstraintLayout`.
- One way to position a `View` is with a margin.
- A margin says how far a `View` is from an edge of the container it's in.
- You can set attributes on a `TextView` like the font, text size, and color.

#### [Add images to your Android app](https://developer.android.com/codelabs/basic-android-kotlin-training-birthday-card-app-image)

In this codelab you will learn how to add images to your app using an `ImageView`.

- The **Resource Manager** in Android Studio helps you add and organize your images and other resources.
- An `ImageView` is a UI element for displaying images in your app.
- `ImageViews` should have a content description to help make your app more accessible.
- Text that is shown to the user like the birthday greeting should be extracted into a string resource to make it easier to translate your app into other languages.

### [Android Basics: Add a button to an app](https://developer.android.com/courses/pathways/android-basics-kotlin-four)

Learn how to use classes, objects, and conditionals to create an interactive app for your users.

#### [Classes and object instances in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-create-dice-roller-in-kotlin)

In this first codelab, you will create a Kotlin program that simulates rolling dice and outputs a random number, just like a dice would.

- Call the `random()` function on an `IntRange` to generate a random number: `(1..6).random()`
- Classes are like a blueprint of an object. They can have properties and behaviors, implemented as variables and functions.
- An instance of a class represents an object, often a physical object, such as a dice. You can call the actions on the object and change its attributes.
- You can supply values to a class when you create an instance. For example: `class Dice(val numSides: Int)` and then create an instance with `Dice(6)`.
- Functions can return something. Specify the data type to be returned in the function definition, and use a `return` statement in the function body to return something. For example: `fun example(): Int { return 5 }`

#### [Create an interactive Dice Roller app](https://developer.android.com/codelabs/basic-android-kotlin-training-create-dice-roller-app-with-button)

In this codelab, you will create a Dice Roller Android app where users can click a `Button` in the app to roll a dice. The outcome of the roll will be shown in a `TextView` on the screen.

- Add a `Button` in an Android app using the **Layout Editor**.
- Modify the `MainActivity.kt` class to add interactive behavior to the app.
- Pop up a `Toast` message as a temporary solution to verify you're on the right track.
- Set an on-click listener for a `Button` using `setOnClickListener()` to add behavior for when a `Button` is clicked.
- When the app is running, you can update the screen by calling methods on the `TextView`, `Button`, or other UI elements in the layout.
- Comment your code to help other people who are reading your code understand what your approach was.
- Reformat your code and clean up your code.

#### [Add conditional behavior in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-conditional-dice-roll-behavior)

In this Kotlin codelab you will create another dice game, Lucky Dice Roll, trying to roll a lucky number. Your program will set a lucky number and roll the dice. You then check the roll against the lucky number and print an appropriate message to the output. To accomplish this, you will learn how to compare values and make different decisions in your Kotlin program.

- Use an `if` statement to set a condition for executing some instructions. For example, if the user rolls the lucky number, print a winning message.
- The `Boolean` data type has values of `true` and `false` and can be used for decision making.
- Compare values using operators such as greater than (`>`), less than (`<`), and equal to (`==`).
- Use a chain of `else if` statements to set multiple conditions. For example, print a different message for each possible dice roll.
- Use an `else` statement at the end of a chain of conditions to catch any cases that may not be covered explicitly. If you cover the cases for 6-sided dice, an `else` statement would catch the 7 and 8 numbers rolled with an 8-sided dice.
- Use a `when` statement as a compact form of executing code based on comparing a value.

#### [Add images to the Dice Roller app](https://developer.android.com/codelabs/basic-android-kotlin-training-dice-roller-images)

- Use [`setImageResource()`](https://developer.android.com/reference/android/widget/ImageView#setImageResource(int)) to change the image that's displayed in an `ImageView`
- Use control flow statements like `if / else` expressions or `when` expressions to handle different cases in your app, for example, showing different images under different circumstances.