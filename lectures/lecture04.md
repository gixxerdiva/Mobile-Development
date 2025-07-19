# Lecture 4 – Android UI Layouts and Views

**Course**: ISTM 6216 – Mobile Applications Development  
**Instructor**: Dr. Anya Mendenhall  
**Semester**: Fall 2025  
**Topic**: Layout Design, XML, ViewGroups, and Basic UI Components

---

## 🎯 Objectives

- Understand the structure of Android UI design  
- Use XML to define layouts  
- Learn about Views and ViewGroups  
- Explore key UI components (TextView, EditText, Button, ImageView)  
- Practice building interfaces using the Layout Editor and XML

---

## 🧠 Topics Covered

### 1. What is a Layout?
- A layout defines the visual structure for a UI screen
- Can be created using **XML** or programmatically in Kotlin
- The root element is typically a `ViewGroup`

---

### 2. View vs ViewGroup
- **View**: a basic UI component (e.g., TextView, Button)
- **ViewGroup**: a container that holds multiple views (e.g., LinearLayout, ConstraintLayout)

---

### 3. Layout Types

#### ➤ LinearLayout
- Arranges child views **vertically** or **horizontally**
- Attributes: `orientation`, `layout_width`, `layout_height`

#### ➤ RelativeLayout (Deprecated)
- Positions views relative to each other or the parent
- Superseded by ConstraintLayout

#### ➤ ConstraintLayout
- Modern, flexible layout manager
- Uses **constraints** for precise positioning
- Supports flat layout hierarchies = better performance

---

### 4. Common View Elements

- `TextView` – displays text  
- `EditText` – allows user input  
- `Button` – performs actions on tap  
- `ImageView` – displays images  
- `CheckBox`, `RadioButton`, `Switch` – input toggles  

Example:
```xml
<TextView
  android:id="@+id/greetingText"
  android:layout_width="wrap_content"
  android:layout_height="wrap_content"
  android:text="Hello, Android!" />

