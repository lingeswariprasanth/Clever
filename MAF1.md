# Flutter Project Setup and Running a Basic App on Emulator
## **1. Create a New Flutter Project**

### **Steps to Create a Flutter Project**:

1. **Install Flutter SDK**:
   - Follow the [official Flutter installation guide](https://flutter.dev/docs/get-started/install).

2. **Set Up Flutter Environment**:
   - Ensure Flutter is added to your system's PATH.
   - Verify installation by running:
     ```bash
     flutter doctor
     ```

3. **Create a New Project**:
   - Run the following command in your terminal or command prompt:
     ```bash
     flutter create my_first_app
     ```
   - Navigate into the project directory:
     ```bash
     cd my_first_app
     ```

---

## **2. Explore the Flutter Project Folder Structure**

### **Key Folders and Files**:

1. **`lib/`**
   - Contains the main source code for your app.
   - Default file: `main.dart`.

2. **`test/`**
   - Contains test files for writing unit and widget tests.

3. **`android/`**
   - Contains Android-specific files for the project.

4. **`ios/`**
   - Contains iOS-specific files for the project.

5. **`pubspec.yaml`**
   - A configuration file for dependencies, assets, and project metadata.

6. **`build/`**
   - Contains the output files generated during the build process.

7. **`web/` (Optional)**
   - Contains web-specific files if the web platform is enabled.

---

## **3. Running a Basic Flutter App on Emulator**

### **Steps**:

1. **Install an Emulator**:
   - For Android:
     - Open Android Studio.
     - Go to **Tools > AVD Manager** and create a virtual device.
     - Start the emulator.

2. **Run the App**:
   - Ensure the emulator is running.
   - Run the following command in the project directory:
     ```bash
     flutter run
     ```
   - The app will launch on the emulator with a default **"Counter App"**.

3. **Modify the App**:
   - Open `lib/main.dart` and edit the `MyHomePage` widget to customize the app.

---

## **4. Sample Code for Basic Flutter App**

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('My First Flutter App'),
        ),
        body: Center(
          child: Text('Hello, Flutter!'),
        ),
      ),
    );
  }
}
```

### **Steps to Run the Modified App**:
1. Save the changes in `main.dart`.
2. Run `flutter run` again or press **R** to hot reload if the app is already running.

---

## **5. Common Commands for Flutter Development**

- **Run the app**:
  ```bash
  flutter run
  ```

- **Check for issues**:
  ```bash
  flutter doctor
  ```

- **Add a dependency**:
  ```bash
  flutter pub add <package_name>
  ```

- **Get all dependencies**:
  ```bash
  flutter pub get
  ```

- **Hot reload (while app is running)**:
  Press **R** in the terminal.

---


