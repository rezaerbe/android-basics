# [Android Basics in Kotlin](https://developer.android.com/courses/android-basics-kotlin/course)

Welcome to Android Basics in Kotlin! In this course, you'll learn the basics of building Android apps with the Kotlin programming language. Along the way, you'll develop a collection of apps to start your journey as an Android developer.

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