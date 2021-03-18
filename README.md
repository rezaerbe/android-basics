# [Android Basics in Kotlin](https://developer.android.com/courses/android-basics-kotlin/course)

Welcome to Android Basics in Kotlin! In this course, you'll learn the basics of building Android apps with the Kotlin programming language. Along the way, you'll develop a collection of apps to start your journey as an Android developer.

### Happy Birthday App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/HappyBirthday.jpg?raw=true" width=250 />

### Dice Roller App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/DiceRoller.jpg?raw=true" width=250 />

### Calculator App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Calculator.jpg?raw=true" width=250 />

### Affirmation App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Affirmation.jpg?raw=true" width=250 />

### Word App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Word1.jpg?raw=true" width=250 /> &nbsp; <img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Word2.jpg?raw=true" width=250 /> &nbsp; <img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Word3.jpg?raw=true" width=250 />

### Unscramble App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Unscramble1.jpg?raw=true" width=250 /> &nbsp; <img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Unscramble2.jpg?raw=true" width=250 />

### Cupcake App

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Cupcake1.jpg?raw=true" width=250 /> &nbsp; <img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Cupcake2.jpg?raw=true" width=250 />

<img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Cupcake3.jpg?raw=true" width=250 /> &nbsp; <img src="https://raw.githubusercontent.com/rezaerbe/android-basics/master/Screenshot/Cupcake4.jpg?raw=true" width=250 />

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

## [Unit 2: Layouts](https://developer.android.com/courses/android-basics-kotlin/unit-2)

Improve the user interface of your app by learning about layouts, Material Design guidelines, and best practices for UI development.

### [Get user input in an app: Part 1](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-2-pathway-1)

Create a tip calculator app by building the layout first, then implement the logic to calculate the tip from the user input.

#### [Classes and inheritance in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-classes-and-inheritance)

In this codelab you learned how to:

- Create a class hierarchy, that is a tree of classes where children inherit functionality from parent classes. Properties and functions are inherited by subclasses.
- Create an `abstract` class where some functionality is left to be implemented by its subclasses. An `abstract` class can therefore not be instantiated.
- Create subclasses of an `abstract` class.
- Use `override` keyword to override properties and functions in subclasses.
- Use the `super` keyword to reference functions and properties in the parent class.
- Make a class `open` so that it can be subclassed.
- Make a property `private`, so it can only be used inside the class.
- Use the `with` construct to make multiple calls on the same object instance.
- Import functionality from the `kotlin.math` library

#### [Create XML layouts for Android](https://developer.android.com/codelabs/basic-android-kotlin-training-xml-layouts)

In this codelab, you will be building the layout for a basic tip calculator app. At the end of the codelab, you'll have a working UI for the app, but the app won't actually calculate the tip yet. Making the app work and look more professional will be in the following codelabs.

- XML (Extensible Markup Language) is a way of organizing text, made of tags, elements, and attributes.
- Use XML to define the layout of an Android app.
- Use `EditText` to let the user input or edit text.
- An `EditText` can have a hint to tell the user what is expected in that field.
- Specify the `android:inputType` attribute to limit what type of text the user can input into an `EditText` field.
- Make a list of exclusive options with `RadioButtons`, grouped with a `RadioGroup`.
- A `RadioGroup` can be vertical or horizontal, and you can specify which `RadioButton` should be selected initially.
- Use a `Switch` to let the user toggle between two options.
- You can add a label to a `Switch` without using a separate `TextView`.
- Each child of a `ConstraintLayout` needs to have vertical and horizontal constraints.
- Use "start" and "end" constraints to handle both Left to Right (LTR) and Right to Left (RTL) languages.
- Names of the constraint attributes follow the form `layout_constraint<Source>_to<Target>Of`.
- To make a `View` as wide as the `ConstraintLayout` it's in, constrain the start and end to the start and end of the parent, and set the width to 0dp.

#### [Calculate the tip](https://developer.android.com/codelabs/basic-android-kotlin-training-tip-calculator)

In this codelab, you will be writing code for the tip calculator to go with the UI you created in the previous codelab, Create XML layouts for Android.

- View binding lets you more easily write code that interacts with the UI elements in your app
- The `Double` data type in Kotlin can store a decimal number
- Use the `checkRadioButtonId` attribute of a `RadioGroup` to find which `RadioButton` is selected
- Use `NumberFormat.getCurrencyInstance()` to get a formatter to use for formatting numbers as currency
- You can use string parameters like `%s` to create dynamic strings that can still be easily translated into other languages
- Testing is important!
- You can use **Logcat** in Android Studio to troubleshoot problems like the app crashing
- A stack trace shows a list of methods that were called. This can be useful if the code generates an exception.
- Exceptions indicate a problem that code didn't expect
- `Null` means "no value"
- Not all code can handle `null` values, so be careful using it
- Use **Analyze > Inspect Code** for suggestions to improve your code

### [Get user input in an app: Part 2](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-2-pathway-2)

Add visual polish to the Tip Calculator app to create a better user experience.

#### [Change the app icon](https://developer.android.com/codelabs/basic-android-kotlin-training-change-app-icon)

This codelab will provide you with image source files for a Tip Calculator launcher icon to practice with. You will use a tool in Android Studio called Image Asset Studio to generate all versions of the launcher icons needed. Afterwards, you can take what you learned and apply it to changing the app icon for other apps!

- Place app icon files in the `mipmap` resource directories.
- Provide different versions of an app icon bitmap image in each density bucket (`mdpi`, `hdpi`, `xhdpi`, `xxhdpi`, `xxxhdpi`) for backwards compatibility with older versions of Android.
- Add resource qualifiers onto resource directories to specify resources that should be used on devices with a certain configuration (e.g. `v26`).
- Vector drawables are Android's implementation of vector graphics. They are defined in XML as a set of points, lines, and curves along with associated color information. Vector drawables can be scaled for any density without loss of quality.
- Adaptive icons were introduced to the Android platform in API 26. They are made up of a foreground and background layer that follow specific requirements, so that your app icon looks high-quality on a range of devices with different OEM masks.
- Use Image Asset Studio in Android Studio to create legacy and adaptive icons for your app.

#### [Create a more polished user experience](https://developer.android.com/codelabs/basic-android-kotlin-training-polished-user-experience)

In this codelab, you will update the tip calculator app (from [previous codelabs](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-2-pathway-1)) to have a more polished user experience, as seen in the final screenshot below. You'll also test the app in some additional scenarios to ensure the user experience is as smooth as possible.

- Use Material Design Components where possible to adhere to Material Design guidelines and allow for more customization.
- Add icons to give users visual cues about how parts of your app will function.
- Use `ConstraintLayout` to position elements in your layout.
- Test your app for edges cases (e.g. rotating your app in landscape mode) and make improvements where applicable.
- Comment your code to help other people who are reading your code understand what your approach was.
- Reformat your code and clean up your code to make it as concise as possible.

### [Display a scrollable list](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-2-pathway-3)

Create an app that displays a scrollable list of inspiring text and images using the RecyclerView widget in Android. Along the way, you’ll learn about using lists in Kotlin to store a collection of data.

#### [Use Lists in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-lists)

In this codelab, you will use the Kotlin Playground to become familiar with lists in Kotlin and create a program for ordering different variations of noodle soup.

- A list is an ordered collection of elements of a specific type, such as a list of `Strings.`
- The index is the integer position that reflects the position of the element (e.g. `myList[2]`).
- In a list, the first element is at index 0 (e.g. `myList[0]`), and the last element is at `myList.size-1` (e.g. `myList[myList.size-1]` or `myList.last()`).
- There are two types of lists: `List` and `MutableList.`
- A `List` is read-only and cannot be modified once it has been initialized. However, you can apply operations such as `sorted()` and `reversed()` which return a new list without changing the original.
- A `MutableList` can be modified after creation such as adding, removing, or modifying elements.
- You can add a list of items to a mutable list using `addAll()`.
- Use a `while` loop to execute a block of code until the expression evaluates to false and you exit the loop.

#### [Use RecyclerView to display a scrollable list](https://developer.android.com/codelabs/basic-android-kotlin-training-recyclerview-scrollable-list)

In this codelab, you will build the Affirmations app. Affirmations is a simple app that displays ten positive affirmations as text in a scrolling list. Then, in the follow-up codelab, you will take it a step further, add an inspiring image to each affirmation, and polish the app UI.

- `RecyclerView` widget helps you display a list of data.
- `RecyclerView` uses the adapter pattern to adapt and display the data.
- `ViewHolder` creates and holds the views for `RecyclerView`.
- `RecyclerView` comes with built in `LayoutManagers`. `RecyclerView` delegates how items are laid out to `LayoutManagers`.

To implement the adapter:

- Create a new class for the adapter, for example, `ItemAdapter`.
- Create a custom `ViewHolder` class that represents a single list item view. Extend from `RecyclerView.ViewHolder` class.
- Modify the `ItemAdapter` class to extend from the `RecyclerView`.`Adapter` class with the custom `ViewHolder` class.
- Implement these methods within the adapter: `getItemsCount()`, `onCreateViewHolder()`, and `onBindViewHolder()`.

#### [Display a list of images using cards](https://developer.android.com/codelabs/basic-android-kotlin-training-display-list-cards)

In this follow-up codelab, you add an inspiring image to each affirmation of your app. You will display the text and image for each affirmation within a card, using the `MaterialCardView` widget from the Material Components for Android library. Then you will finish the app by polishing the UI to create a more cohesive and beautiful user experience.

- To display additional content in a `RecyclerView`, modify the underlying data model class and data source. Then update the list item layout and adapter to set that data onto the views.
- Use resource annotations to help ensure that the right type of resource ID is passed into a class constructor.
- Use the **Material Components for Android library** to have your app more easily follow the recommended Material Design guidelines.
- Use `MaterialCardView` to display content in a Material card.
- Small visual tweaks to your app in terms of color and spacing can make the app look more polished and consistent.

## [Unit 3: Navigation](https://developer.android.com/courses/android-basics-kotlin/unit-3)

Enhance your users’ ability to navigate across, into and back out from the various screens within your app for a consistent and predictable user experience.

### [Navigate between screens](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-3-pathway-1)

Add another screen to an app by adding a second activity, and use an intent to navigate to it. Also, learn the basics of the activity lifecycle as you navigate into and out of different activities.

#### [Collections in Kotlin](https://developer.android.com/codelabs/basic-android-kotlin-training-collections)

In this codelab you will learn more about collections, and about lambdas and higher-order functions in Kotlin.

- A collection is a group of related items
- Collections can be mutable or immutable
- Collections can be ordered or unordered
- Collections can require unique items or allow duplicates
- Kotlin supports different kinds of collections including lists, sets, and maps
- Kotlin provides many functions for processing and transforming collections, including `forEach`, `map`, `filter`, `sorted`, and more.
- A lambda is a function without a name that can be passed as an expression immediately. An example would be { a: Int -> a * 3 }.
- A higher-order function means passing a function to another function, or returning a function from another function.

#### [Activities and Intents](https://developer.android.com/codelabs/basic-android-kotlin-training-activities-intents)

In this codelab, you'll build out a dictionary app so that it uses multiple activities, uses intents to navigate between them, and passes data to other apps.

- Explicit intents are used to navigate to specific activities in your app.
- Implicit intents correspond to specific actions (like opening a link, or sharing an image) and let the system determine how to fulfill the intent.
- Menu options allow you to add buttons and menus to the app bar.
- Companion objects provide a way to associate reusable constants with a type, rather than an instance of that type.

To perform an intent:

- Get a reference to the context.
- Create an `Intent` object providing either an activity or intent type (depending on whether it's explicit or implicit).
- Pass any needed data by calling `putExtra()`.
- Call `startActivity()` passing in the `intent` object.

#### [Stages of the activity lifecycle](https://developer.android.com/codelabs/basic-android-kotlin-training-activity-lifecycle)

In this codelab, you learn more about a fundamental part of Android: the *activity*. The *activity lifecycle* is the set of states an activity can be in during its lifetime. The lifecycle extends from when the activity is initially created to when it is destroyed and the system reclaims that activity's resources. As a user navigates between activities in your app (and into and out of your app), those activities each transition between different states in the activity lifecycle.

##### Activity lifecycle

- The *activity lifecycle* is a set of states through which an activity migrates. The activity lifecycle begins when the activity is first created and ends when the activity is destroyed.
- As the user navigates between activities and inside and outside of your app, each activity moves between states in the activity lifecycle.
- Each state in the activity lifecycle has a corresponding callback method you can override in your `Activity` class. The core set of lifecycle methods are: [`onCreate()`](https://developer.android.com/reference/android/app/Activity.html#onCreate(android.os.Bundle))[`onStart()`](https://developer.android.com/reference/android/app/Activity.html#onStart())[`onPause()`](https://developer.android.com/reference/android/app/Activity.html#onPause())[`onRestart()`](https://developer.android.com/reference/android/app/Activity.html#onRestart())[`onResume()`](https://developer.android.com/reference/android/app/Activity.html#onResume())[`onStop()`](https://developer.android.com/reference/android/app/Activity.html#onStop())[`onDestroy()`](https://developer.android.com/reference/android/app/Activity.html#onDestroy())
- To add behavior that occurs when your activity transitions into a lifecycle state, override the state's callback method.
- To add skeleton override methods to your classes in Android Studio, select **Code > Override Methods** or press `Control+o` (`Command+o` on Mac)

##### Logging with Log

- The Android logging API, and specifically the [`Log`](https://developer.android.com/reference/android/util/Log) class, enables you to write short messages that are displayed in the Logcat within Android Studio.
- Use `Log.d()` to write a debug message. This method takes two arguments: the log *tag*, typically the name of the class, and the log *message*, a short string.
- Use the **Logcat** window in Android Studio to view the system logs, including the messages you write.

##### Preserving activity state

- When your app goes into the background, just after `onStop()` is called, app data can be saved to a bundle. Some app data, such as the contents of an `EditText`, is automatically saved for you.
- The bundle is an instance of [`Bundle`](https://developer.android.com/reference/kotlin/android/os/Bundle), which is a collection of keys and values. The keys are always strings.
- Use the `onSaveInstanceState()` callback to save other data to the bundle that you want to retain, even if the app was automatically shut down. To put data into the bundle, use the bundle methods that start with `put`, such as `putInt()`.
- You can get data back out of the bundle in the `onRestoreInstanceState()` method, or more commonly in `onCreate()`. The `onCreate()` method has a `savedInstanceState` parameter that holds the bundle.
- If the `savedInstanceState` variable is `null`, the activity was started without a state bundle and there is no state data to retrieve.
- To retrieve data from the bundle with a key, use the `Bundle` methods that start with `get`, such as `getInt()`.

##### Configuration changes

- A *configuration change* happens when the state of the device changes so radically that the easiest way for the system to resolve the change is to destroy and rebuild the activity.
- The most common example of a configuration change is when the user rotates the device from portrait to landscape mode, or from landscape to portrait mode. A configuration change can also occur when the device language changes or a hardware keyboard is plugged in.
- When a configuration change occurs, Android invokes all the activity lifecycle's shutdown callbacks. Then Android restarts the activity from scratch, running all the lifecycle startup callbacks.
- When Android shuts down an app because of a configuration change, it restarts the activity with the state bundle that is available to `onCreate()`.
- As with process shutdown, save your app's state to the bundle in `onSaveInstanceState()`.

### [Introduction to the Navigation component](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-3-pathway-2)

Learn how to simplify in-app screen navigation with the Navigation component, a collection of libraries, useful tooling and best practices.

#### [Fragments and the Navigation Component](https://developer.android.com/codelabs/basic-android-kotlin-training-fragments-navigation-component)

In the Activities and Intents codelab, you added intents in the [Words](https://github.com/google-developer-training/android-basics-kotlin-words-app/tree/activities) app, to navigate between two activities. While this is a useful navigation pattern to know, it's only part of the story of making dynamic user interfaces for your apps. Many Android apps don't need a separate activity for every screen. In fact, many common UI patterns, such as tabs, exist within a single activity, using something called *fragments*.

- Fragments are reusable pieces of UI that can be embedded in activities.
- The lifecycle of a fragment differs from the lifecycle of an activity, with view setup occurring in `onViewCreated()`, rather than `onCreateView()`.
- A `FragmentContainerView` is used to embed fragments in other activities and can manage navigation between fragments.

Using the Navigation Component

- Setting the `navGraph` attribute of a `FragmentContainerView` allows you to navigate between fragments within an activity.
- The `NavGraph` editor allows you to add navigation actions and specify arguments between different destinations.
- While navigating using intents requires you to pass in extras, the Navigation component uses SafeArgs to auto-generate classes and methods for your navigation actions, ensuring type safety with arguments.

Use cases for fragments.

- Using the Navigation component, many apps can manage their entire layout within a single activity, with all navigation occurring between fragments.
- Fragments make common layout patterns possible, such as master-detail layouts on tablets, or multiple tabs within the same activity.

### [Architecture components](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-3-pathway-3)

Learn how to use Android Jetpack Architecture components, a collection of libraries that help you design robust, testable, and maintainable apps.

#### [Store data in ViewModel](https://developer.android.com/codelabs/basic-android-kotlin-training-viewmodel)

In this codelab, you learn how to use [`ViewModel`](https://developer.android.com/topic/libraries/architecture/viewmodel), one of the Architecture components to store your app data. The stored data is not lost if the framework destroys and re-creates the activities and fragments during a configuration change or other events.

- The Android app architecture guidelines recommend separating classes that have different responsibilities and driving the UI from a model.
- A UI controller is a UI-based class like `Activity` or `Fragment`. UI controllers should only contain logic that handles UI and operating system interactions; they shouldn't be the source of data to be displayed in the UI. Put that data and any related logic in a `ViewModel`.
- The `ViewModel` class stores and manages UI-related data. The `ViewModel` class allows data to survive configuration changes such as screen rotations.
- `ViewModel` is one of the recommended Android Architecture Components.

#### [Use LiveData with ViewModel](https://developer.android.com/codelabs/basic-android-kotlin-training-livedata)

In this codelab, you'll learn how to integrate [`LiveData`](https://developer.android.com/reference/android/arch/lifecycle/LiveData.html) with the data in the `ViewModel`.

- `LiveData` holds data; `LiveData` is a wrapper that can be used with any data
- `LiveData` is observable, which means that an observer is notified when the data held by the `LiveData` object changes.
- `LiveData` is lifecycle-aware. When you attach an observer to the `LiveData`, the observer is associated with a [`LifecycleOwner`](https://developer.android.com/topic/libraries/architecture/lifecycle#lco) (usually an Activity or Fragment). The LiveData only updates observers that are in an active lifecycle state such as [`STARTED`](https://developer.android.com/reference/android/arch/lifecycle/Lifecycle.State.html#STARTED) or [`RESUMED`](https://developer.android.com/reference/android/arch/lifecycle/Lifecycle.State.html#RESUMED). You can read more about `LiveData` and observation [here](https://developer.android.com/topic/libraries/architecture/livedata.html#work_livedata).
- Apps can listen to the LiveData changes from the layout using Data Binding and binding expressions.
- Binding expressions are written within the layout in the attribute properties (such as `android:text`) referencing the layout properties.

### [Advanced navigation app examples](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-3-pathway-4)

Combine everything you've learned in this unit about navigation, view model, data binding, and live data by building a more advanced app that also includes custom back stack behavior.

#### [Shared ViewModel Across Fragments](https://developer.android.com/codelabs/basic-android-kotlin-training-shared-viewmodel)

 In this codelab, you will put everything together and work on an advanced sample, a cupcake ordering app. You will learn how to use a [shared `ViewModel`](https://developer.android.com/topic/libraries/architecture/viewmodel.html#sharing) to share data between the fragments of the same activity and new concepts like `LiveData` transformations.

- The [`ViewModel`](https://developer.android.com/topic/libraries/architecture/viewmodel) is a part of the [Android Architecture Components](https://developer.android.com/topic/libraries/architecture) and the app data saved within the `ViewModel` is retained during configuration changes. To add a `ViewModel` to your app, you create a new class and extend it from the [`ViewModel`](https://developer.android.com/topic/libraries/architecture/viewmodel) class.
- [Shared `ViewModel`](https://developer.android.com/topic/libraries/architecture/viewmodel.html#sharing) is used to save the app's data from multiple fragments in a single `ViewModel`. Multiple fragments in the app will access the shared `ViewModel` using their activity scope.
- [`LifecycleOwner`](https://developer.android.com/reference/androidx/lifecycle/LifecycleOwner) is a class that has an Android lifecycle, such as an activity or a fragment.
- `LiveData` observer observes the changes to the app's data only if the lifecycle owner is in active states (`STARTED` or `RESUMED`).
- Listener bindings are lambda expressions that run when an event happens such as an `onClick` event. They are similar to method references such as `textview.setOnClickListener(clickListener)` but listener bindings let you run arbitrary data binding expressions.
- The `LiveData` transformation method(s) provides a way to perform data manipulations on the source `LiveData` and return a resulting `LiveData` object.
- Android frameworks provides a class called [`SimpleDateFormat`](https://developer.android.com/reference/java/text/SimpleDateFormat), a class for formatting and parsing dates in a locale-sensitive manner. It allows for formatting (date → text) and parsing (text → date) dates.

#### [Navigation and the back stack](https://developer.android.com/codelabs/basic-android-kotlin-training-navigation-backstack)

In this codelab, you'll finish implementing the rest of the **Cupcake** app, which you started in a previous codelab. The **Cupcake** app has multiple screens and shows an order flow for cupcakes. The completed app should allow the user to navigate through the app.

- Android keeps a back stack of all the destinations you've visited, with each new destination being pushed onto the stack.
- By tapping the **Up** or **Back** button, you can pop destinations off the back stack.
- Using the Jetpack Navigation component helps you push and pop fragment destinations off the back stack, so that the default **Back** button behavior comes for free.
- Specify the `app:popUpTo` attribute on an action in the navigation graph, in order to pop destinations off the back stack until the specified one in the attribute value.
- Specify `app:popUpToInclusive="true"` on an action when the destination specified in `app:popUpTo` should also be popped off the back stack.
- You can create an implicit intent to share content to an email app, using `Intent.ACTION_SEND` and populating intent extras such as `Intent.EXTRA_EMAIL`, `Intent.EXTRA_SUBJECT`, and `Intent.EXTRA_TEXT` to name a few.
- Use a `plurals` resource if you want to use different string resources based on quantity, such as the singular or plural case.