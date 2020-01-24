# Flutter Interview Questions and Answers

Flutter is booming in the mobile market as the next revolution. It has proven to hold the potential to win over every mobile technology and become the only choice for cross-platform app development in the future. Follow along and check the first most comprehensive list of Flutter Interview Questions and Answers that will trend on mobile developers interviews in 2020. 

> You could find all the answers here 👉 https://www.fullstack.cafe/Flutter.

<p align="center">
  <a href="https://www.fullstack.cafe">
  <img src="https://user-images.githubusercontent.com/13550565/73042889-e7533900-3e9d-11ea-94f2-b4a9e87cc018.png">
  </a>
</p>

### Q1: What is Flutter? ⭐

**Answer:**

**Flutter** is an open-source UI toolkit from *Google* for crafting beautiful, natively compiled applications for desktop, web, and mobile from a single codebase. Flutter apps are built using the *Dart* programming language.


🔗 **Source:** [flutter.dev](https://flutter.dev)


### Q2: When to use main Axis Alignment and cross Axis Alignment? ⭐

**Answer:**

**For Row:**  
`mainAxisAlignment` = Horizontal Axis   
`crossAxisAlignment` = Vertical Axis

![enter image description here](https://i.stack.imgur.com/aypHr.png)

**For Column:**
  
`mainAxisAlignment` = Vertical Axis      
`crossAxisAlignment` = Horizontal Axis

![enter image description here](https://i.stack.imgur.com/eseWF.png)


[Image source](https://flutter.dev/docs/development/ui/layout#aligning-widgets)

🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/53850149/flutter-crossaxisalignment-vs-mainaxisalignment/53856933#53856933)


### Q3: What is Dart and why does Flutter use it? ⭐⭐

**Answer:**

**Dart** is an *object-oriented*, *garbage-collected* programming language that you use to develop Flutter apps.
It was also created by Google, but is open-source, and has community inside and outside Google.
Dart was chosen as the language of **Flutter** for the following reason: 
- Dart is **AOT** (Ahead Of Time) compiled to fast, predictable, native code, which allows almost all of Flutter to be written in Dart. This not only makes Flutter fast, virtually everything (including all the widgets) can be customized.
- Dart can also be **JIT** (Just In Time) compiled for exceptionally fast development cycles and game-changing workflow (including Flutter’s popular sub-second stateful hot reload).
- Dart allows Flutter to avoid the need for a separate declarative layout language like *JSX* or *XML*, or separate visual interface builders, because Dart’s declarative, programmatic layout is easy to read and visualize. And with all the layout in one language and in one place, it is easy for Flutter to provide advanced tooling that makes layout a snap.

🔗 **Source:** [hackernoon.com](https://hackernoon.com/why-flutter-uses-dart-dd635a054ebf)


### Q4: What is a "widget" and mention its importance in Flutter? ⭐⭐

**Answer:**

- Widgets are basically the UI components in Flutter.
- It is a way to describe the configuration of an *Element*.
- They are inspired from components in **React**.

Widgets are important in Flutter because everything within a Flutter application is a  **Widget**  , from a simple “_Text”_  to “_Buttons”_  to “_Screen Layouts”_.

🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/50958238/what-is-a-widget-in-flutter)


### Q5: How many types of widgets are there in Flutter? ⭐⭐

**Answer:**

There are two types of widgets:
1.  **StatelessWidget** : A widget that does not require mutable state.
2.  **StatefulWidget**: A widget that has mutable state.

🔗 **Source:** [proandroiddev.com](https://proandroiddev.com/flutter-from-zero-to-comfortable-6b1d6b2d20e)


### Q6: When should you use WidgetsBindingObserver? ⭐⭐

**Answer:**

WidgetsBindingObserver should be used when we want to listen to the `AppLifecycleState` and call stop/start on our services.

🔗 **Source:** [www.filledstacks.com](https://www.filledstacks.com/post/flutter-application-life-cycle-management/)


### Q7: What is the difference between "main()" and "runApp()" functions in Flutter? ⭐⭐

**Answer:**

- `main ()` function came from *Java*-like languages so it's where all program started, without it, you can't write any program on Flutter even without UI.
- `runApp()` function should return *Widget* that would be attached to the screen as a root of the *Widget Tree* that will be rendered.

🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/58883728/what-is-the-difference-between-main-function-and-the-runapp-function-in-flutte)


### Q8: What is the difference between Expanded and Flexible widgets? ⭐⭐

**Answer:**

`Expanded` is just a shorthand for `Flexible`

Using expanded this way:
```dart
Expanded(
	child: Foo(),
);
```
is strictly equivalent to:
```dart
Flexible(
	fit: FlexFit.tight,
	child: Foo(),
);
```

You may want to use `Flexible` over `Expanded` when you want a different `fit`, useful in some responsive layouts.

The difference between `FlexFit.tight` and `FlexFit.loose` is that loose will allow its child to have a maximum size while tight forces that child to fill all the available space.

🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/52645944/flutter-expanded-vs-flexible)


### Q9: How is Flutter different from a WebView based application? ⭐⭐

**Answer:**

- Code you write for a **WebView** or an app that runs similarly has to go through multiple layers to finally get executed (like Cordova for Ionic).** In essence, Flutter leapfrogs that by **compiling down to native **ARM** code to execute on both platforms. 
- “Hybrid” apps are slow, sluggish and look different from the platform they run on. *Flutter* apps run much, much faster than their hybrid counterparts. 
- It’s much easier to access native components and sensors using plugins rather than using **WebView** which can’t take full use of their platform.

🔗 **Source:** [medium.com](https://medium.com/@dev.n/answering-questions-on-flutter-app-development-6d50eb7223f3)


### Q10: What is the pubspec.yaml file and what does it do? ⭐⭐

**Answer:**

- The `pubspec.yaml` file allows you to define the packages your app relies on, declare your assets like images, audio, video, etc. 
- It allows you to set constraints for your app. 
- For Android developers, this is roughly similar to a `build.gradle` file.

🔗 **Source:** [medium.com](https://medium.com/@dev.n/answering-questions-on-flutter-app-development-6d50eb7223f3)


### Q11: What is an App state?  ⭐⭐

**Answer:**

- State that is not *ephemeral*, that you want to share across many parts of your app, and that you want to keep between user sessions, is what we call **application state** (sometimes also called *shared state*).
- Examples of application state:
	-   User preferences
	-   Login info
	-   Notifications in a social networking app
	-   The shopping cart in an e-commerce app
	-   Read/unread state of articles in a news app

🔗 **Source:** [flutter.dev](https://flutter.dev/docs/development/data-and-backend/state-mgmt/ephemeral-vs-app)


### Q12: What are the different build modes in Flutter? ⭐⭐

**Answer:**

- The Flutter tooling supports three modes when compiling your app, and a headless mode for testing. 
- You choose a compilation mode depending on where you are in the development cycle.
- The modes are:
	- Debug
	- Profile
	- Release

🔗 **Source:** [flutter.dev](https://flutter.dev/docs/testing/build-modes)


### Q13: What is Fat Arrow Notation in Dart and when do you use it? ⭐⭐

**Answer:**

The fat arrow syntax is simply a short hand for returning an expression and is similar to `(){ return expression; }`.

The fat arrow is for returning a single line, braces are for returning a code block.

Only an expression—not a statement—can appear between the arrow (`=>`) and the semicolon (`;`). For example, you can’t put an *if* statement there, but you can use a *conditional* expression
```dart
// Normal function
void function1(int a) {
  if (a == 3) {
    print('arg was 3');
  } else {
    print('arg was not 3');
  }
}

// Arrow Function
void function2(int a) => print('arg was ${a == 3 ? '' : 'not '}3');
```


🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/51868395/flutter-dart-difference-between-and/51869508)


### Q14: Does Flutter work like a browser? How is it different from a WebView based application? ⭐⭐

**Answer:**

To answer this question simply: **Code you write for a WebView or an app that runs similarly has to go through multiple layers to finally get executed.** In essence, Flutter leapfrogs that by **compiling down to native ARM** code to execute on both platforms. “Hybrid” apps are slow, sluggish and look different from the platform they run on. Flutter apps run much, much faster than their hybrid counterparts. Also, it’s much easier to access native components and sensors using plugins rather than using WebViews which can’t take full use of their platform.

🔗 **Source:** [medium.com](https://medium.com/@dev.n/answering-questions-on-flutter-app-development-6d50eb7223f3)


### Q15: What is the pubspec.yaml file and what does it do? ⭐⭐

**Answer:**

The `Pubspec.yaml` allows you to define the packages your app relies on, declare your assets like images, audio, video, etc. It also allows you to set constraints for your app. For Android developers, this is roughly similar to a `build.gradle` file, but the differences between the two are also evident.

🔗 **Source:** [medium.com](https://medium.com/@dev.n/answering-questions-on-flutter-app-development-6d50eb7223f3)


### Q16: When do we use double.INFINITY? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q17: Differentiate  StatelessWidget and StatefulWidget? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q18: Why do we pass functions to widgets? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q19: Differentiate between Hot Restart and Hot Reload? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q20: Explain Navigator Widget and its push pop functions in Flutter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q21: Differentiate between required and optional parameters in Dart? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q22: Differentiate between named parameters and positional parameters in Dart? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q23: What is ScopedModel / BLoC Pattern? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q24: What is Streams in Flutter/Dart? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q25: Explain the different types of Streams? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q26: Why is the build() method on State and not Stateful Widget? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q27: What are packages and plugins in Flutter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q28: What are keys in Flutter and when to use it? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q29: Do you know what Ephemeral state means?  ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q30: What are Null-aware operators? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q31: What is debug mode and when do you use it? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q32: What is profile mode and when do you use it? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q33: What is release mode and when do you use it? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q34: How would you execute code only in debug mode? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q35: How is InheritedWidget different from Provider? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q36: What are some pros of Flutter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q37: Name some cons of using Flutter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q38: Where are the layout files? Why doesn’t Flutter have layout files? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q39: What are some pros and cons of Scoped Model vs BLoC and vice versa? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q40: Explain async, await in Flutter/Dart? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q41: What is Future in Flutter/Dart? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q42: What are the similarities and differences of Future and Stream? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q43: What are Global Keys? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q44: What is a MediaQuery in Flutter and when do we use it? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q45: What is the difference between double.INFINITY and MediaQuery? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q46: When would you use App state or Ephemeral state over another?  ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q47: How does Dart AOT work? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q48: Why should you use kReleaseMode instead of assert? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q49: What is the purpose of SafeArea in Flutter? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q50: What is a difference between these operators "?? and ?." ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q51: List some approaches for State management in Flutter ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q52: Explain Stateful Widget Lifecycle in details ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q53: Why Are StatefulWidget and State Separate Classes? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**


### Q54: What is the difference between debug mode and profile mode? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Flutter)**




