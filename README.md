# Flutter important notes

onPressed property expects a function to be executed when the button is pressed, so fav.remove(word) cannot be used directly: The onPressed property of a button widget in Flutter expects a function that will be executed when the button is pressed. Since fav.remove(word) is not a function but a statement that removes the given word from the fav set, it cannot be used directly. Instead, it needs to be wrapped in a function that takes no arguments and returns nothing.

pubspec.yaml file specifies app's version, dependencies, and assets: The pubspec.yaml file is a YAML file that contains metadata about the app, such as its name, description, version number, author, dependencies, and assets. It's located in the root directory of the app and is used by the Dart package manager (pub) to manage the app's dependencies and assets.

MyApp sets up the app, creates app-wide state, defines the visual theme, and sets the home widget: MyApp is the main widget of the app and is responsible for setting up the app's structure and behavior. It creates the app-wide state object, sets the app's name and visual theme, and specifies the starting point of the app.

MyAppState defines the data needed for the app to function and extends ChangeNotifier to notify others about its own changes: MyAppState is a stateful widget that stores the data needed by the app to function, such as the user's favorite words and the current search query. It extends the ChangeNotifier class to notify other parts of the app when its internal state changes.

MyHomePage tracks changes to the app's current state using the watch method and notifies listeners using notifyListeners() method: MyHomePage is a stateful widget that displays the current state of the app and allows the user to interact with it. It uses the watch method to track changes to the app's current state and updates its own UI whenever the state changes. When a user performs an action that changes the state, MyHomePage calls the notifyListeners() method to notify any widgets that are listening to it that they should update their UI.

Every widget defines a build() method that returns a widget or a nested tree of widgets: In Flutter, every widget must define a build() method that returns a widget or a nested tree of widgets. The build() method is called whenever the widget's circumstances change and should return a new widget that reflects the updated state of the widget.

Scaffold widget is commonly used in real-world Flutter apps: Scaffold is a pre-built widget that provides a standard layout for an app, including an AppBar.
