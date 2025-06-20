# Clothing-Store
# Clothing Store Management System

A JavaFX-based desktop application to manage products, inventory, reviews, and employees in a clothing store.

## Project Path

```
C:\Users\Dell\Desktop\JavaProjects\firstjavafxproject
```

## Team Members and Responsibilities

- **Member 1**: Product Management – Add/edit/delete/view clothing products
- **Member 2**: Inventory Management – Track stock levels and availability
- **Member 3**: Review System – Handle customer feedback and ratings
- **Member 4**: Employee Management – Add/manage employee records


## Requirements

- Java JDK 17 or later
- JavaFX SDK 17.0.2 (or compatible)
- Visual Studio Code with:
  - Java Extension Pack
  - JavaFX configuration (manual or via extension)
- JavaFX SDK extracted in the `lib/` folder or any accessible path

## Folder Structure

- `src/ClothingStore/` – Java source files (main file: `UIFrontend.java`)
- `lib/` – JavaFX SDK libraries
- `bin/` – Output folder for compiled class files (can be created manually or by VS Code)

## How to Compile and Run the Project

### Option 1: Run using Visual Studio Code

1. Open the folder `firstjavafxproject` in VS Code.
2. Make sure your JavaFX SDK is downloaded and stored, e.g., in `lib/javafx-sdk-17.0.2/`.
3. Add VM arguments in `launch.json` (if it doesn't exist, create it in `.vscode/` folder):

```json
{
  "configurations": [
    {
      "type": "java",
      "name": "Launch Clothing Store App",
      "request": "launch",
      "mainClass": "ClothingStore.UIFrontend",
      "vmArgs": "--module-path lib/javafx-sdk-17.0.2/lib --add-modules javafx.controls,javafx.fxml"
    }
  ]
}
```

4. Right-click on `UIFrontend.java` and select **Run Java**.

---

### Option 2: Compile and Run Using Command Line

1. Open Command Prompt (`cmd`).
2. Navigate to your project directory:
```bash
cd "C:\Users\Dell\Desktop\JavaProjects\firstjavafxproject"
```

3. Compile:
```bash
javac --module-path lib\javafx-sdk-17.0.2\lib --add-modules javafx.controls,javafx.fxml -d bin src\ClothingStore\UIFrontend.java
```

4. Run:
```bash
java --module-path lib\javafx-sdk-17.0.2\lib --add-modules javafx.controls,javafx.fxml -cp bin ClothingStore.UIFrontend
```



## Notes

- Make sure all `.java` files are inside the `src/ClothingStore/` directory.
- If you get module path errors, double-check your JavaFX SDK path and version.
- If using IntelliJ or Eclipse instead, configure the JavaFX SDK in the project settings.
