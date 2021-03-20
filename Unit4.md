# [Android Basics in Kotlin](https://developer.android.com/courses/android-basics-kotlin/course)

Welcome to Android Basics in Kotlin! In this course, you'll learn the basics of building Android apps with the Kotlin programming language. Along the way, you'll develop a collection of apps to start your journey as an Android developer.

## [Unit 4: Connect to the internet](https://developer.android.com/courses/android-basics-kotlin/unit-4)

Write coroutines for complex code, and learn about HTTP and REST to get data from the internet.

### [Coroutines](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-4-pathway-1)

Write code for more advanced and complex Android apps.

#### [Introduction to coroutines](https://developer.android.com/codelabs/basic-android-kotlin-training-introduction-coroutines)

In this codelab, you'll learn about threads, and how to use a Kotlin feature called coroutines to write clear, non-blocking concurrent code.

You've learned

- Why concurrency is needed
- What a thread is, and why threads are important for concurrency
- How to write concurrent code in Kotlin using coroutines
- When and when not to mark a function as "suspend"
- The roles of a CoroutineScope, Job, and Dispatcher
- The difference between Deferred and Await

### [Get and display data from the internet](https://developer.android.com/courses/pathways/android-basics-kotlin-unit-4-pathway-2)

Retrieve and display images over the internet with HTTP and REST.

#### [Get data from the internet](https://developer.android.com/codelabs/basic-android-kotlin-training-getting-data-internet)

In this codelab, you use open source developed libraries to build the network layer and get data from a backend server. This greatly simplifies fetching the data, and also helps the app conform to Android best practices, such as performing the operations on a background thread. You will also update the app's user interface if the internet is slow or unavailable; this will keep the user informed about any network connectivity issues.

##### **REST web services**

- A *web service* is software-based functionality offered over the internet that enables your app to make requests and get data back.
- Common web services use a [REST](https://en.wikipedia.org/wiki/Representational_state_transfer) architecture. Web services that offer REST architecture are known as *RESTful* services. RESTful web services are built using standard web components and protocols.
- You make a request to a REST web service in a standardized way, via URIs.
- To use a web service, an app must establish a network connection and communicate with the service. Then the app must receive and parse response data into a format the app can use.
- The [Retrofit](https://square.github.io/retrofit/) library is a client library that enables your app to make requests to a REST web service.
- Use converters to tell Retrofit what to do with data it sends to the web service and gets back from the web service. For example, the `ScalarsConverter` converter treats the web service data as a `String` or other primitive.
- To enable your app to make connections to the internet, add the `"android.permission.INTERNET"` permission in the Android manifest.

##### **JSON parsing**

- The response from a web service is often formatted in [JSON](https://www.json.org/), a common format for representing structured data.
- A JSON object is a collection of key-value pairs.
- A collection of JSON objects is a JSON array. You get a JSON array as a response from a web service.
- The keys in a key-value pair are surrounded by quotes. The values can be numbers or strings.
- The [Moshi](https://github.com/square/moshi) library is an Android JSON parser that converts a JSON string into Kotlin objects. Retrofit has a converter that works with Moshi.
- Moshi matches the keys in a JSON response with properties in a data object that have the same name.
- To use a different property name for a key, annotate that property with the `@Json` annotation and the JSON key name.

#### [Load and display images from the Internet](https://developer.android.com/codelabs/basic-android-kotlin-training-internet-images)

In this codelab, you build on that knowledge to load and display photos from a web URL. You also revisit how to build a `RecyclerView` and use it to display a grid of images on the overview page.

- The [Coil](https://coil-kt.github.io/coil/) library simplifies the process of managing images, such as download, buffer, decode, and cache images in your app.
- [Binding adapters](https://developer.android.com/topic/libraries/data-binding/binding-adapters) are extension methods that sit between a view and that view's bound data. Binding adapters provide custom behavior when the data changes, for example, to call Coil to load an image from a URL into an `ImageView`.
- Binding adapters are extension methods annotated with the `@BindingAdapter` annotation.
- To display a grid of images, use a `RecyclerView` with a `GridLayoutManager`.
- To update the list of properties when it changes, use a binding adapter between the `RecyclerView` and the layout.