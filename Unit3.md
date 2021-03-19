# [Android Basics in Kotlin](https://developer.android.com/courses/android-basics-kotlin/course)

Welcome to Android Basics in Kotlin! In this course, you'll learn the basics of building Android apps with the Kotlin programming language. Along the way, you'll develop a collection of apps to start your journey as an Android developer.

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