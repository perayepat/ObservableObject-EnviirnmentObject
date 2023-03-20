# ObservableObject-EnviirnmentObject
Understanding the difference between observable object and the Environment Object


@ObservedObject in SwiftUI for managing more complex properties that have multiple properties and methods, or that need to be shared across multiple views.

It is similar to @State but uses an external reference type rather than a simple local property. The type used with @ObservedObject should conform to the ObservableObject protocol and can be customized to determine whether changes to each property should force views to refresh or not. 

The easiest way to notify views of changes is by using the @Published property wrapper. Custom publishers from the Combine framework can also be used for more control. When multiple views use an observable object, changes will automatically notify all of them.

<img width="663" alt="Screenshot 2023-03-20 at 15 15 42" src="https://user-images.githubusercontent.com/56199797/226349804-533a3c57-b8fe-47fa-9f20-d1686fe7e316.png">
