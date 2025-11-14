# My Coding Notebook

At the top, begin a table of contents, Ex.:
## Table of Contents
- [Flutter Notes](#flutter-notes)
  - [What is Flutter?](#what-is-flutter)
  - [Key Terms and Definitions](#key-terms-and-definitions)
  - [Layout and Design Widgets](layout-and-design-widgets)
  - [Definitions with Structures](#flutter-definitions)
- [Code Definitions](#code-definitions)


# Flutter Notes

### What is Flutter?
- Definition: A framework made by google for building apps that work on web, Android, and IOS - with one codebase.
- Why is it useful? It saves a lot of time and money, because you can use the code againg

---

### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           |Basic building block of a flutter app Everything is a widget |Text, Image, Container, Column  | 
| MaterialApp      |The root of the app. Setd up routes and themes.   |Found in main.dart                         |
| Scaffold         |Provides basic visual layout -- like a header, is a widget   |                                |
| StatelessWidget  |A widget that can change over time                |Used in MyHomePAge()                       |
| StatefulWidget   |A widget that doesn't change                      |Most of the sreen files                    |
| Navigator        |Manages paths to navigate between screens         |Navigator.pushNamed(context, '/page2' )    |
| AppBar           |                                                  |                                           |
| Column           |                                                  |                                           |
| Row              |                                                  |                                           |
| Container        |                                                  |                                           |
| Text             |Displays text                                     |                                           |
| Image.network    |                                                  |                                           |
---
### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?

---
## Flutter Definitions

| Term | Definition and Description           | Base Structure | Real Life Example | App Example |
|------|--------------------------------------|----------------|-------------------|-------------|
|main()| A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |a chef's recipe|in main.dart, void main() => runApp(MyPortafolioApp()); |
|MaterialApp| The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |the blueprint of a house, for example what color is|return MaterialApp(debugShowCheckedModelBanner: false, title: 'TSA Portfolio', and more |
|Scaffold| A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |Temporary structures in construction that help a person while it isa gradually removed in a contruction|in showcase.dart, return Scaffold( body: Column(mainAxisAligment: MainAxisAlignment.start, children: |
|Column| A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |A column in a store shelv|in showcase.dart, Column(, children: const Padding( padding: EdgeInsets.all(8.0), and more
|Row| A widget that shows things side-by-side. | `Row(...)` |A row in a store shelv|in Infocard.dart, Row, children: ClipRRect, borderRadius: BorderRadius.circular(8),|
|Container| A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |A shelv|background.dart, return Container, width: 160 etc|
|Text| A widget to display text on the screen. | `Text('Hello')` |When you write on a paper|background.dart, Text( title, style: const TextStyle(color: Colors.blue, fontWeight: FontWeight.bold), textAlign: TextAlign.center,  |
|Image.network| A widget to show an image using a link from the internet. | `Image.network('https://...')` |A painting in an art gallery|home.dart, child: Image.network( 'https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQUUKb_E4DWBUWpOJDP_FSA3ZQOgPWoA8uOPOd3zo6TaU0MCXHarhW05900NPFBAVW0c2okk3jAVcMm6xvem1mSUZeYauVNTXAbl8qX0Q', fit: BoxFit.cover,|
|ElevatedButton| A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |Any button|home.dart,  ElevatedButton( onPressed: () => Navigator.pushNamed(context, '/background'),|
|onpressed| The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |when the light is off or on|home.dart, onPressed: () => Navigator.pushNamed(context, '/background'),|
|StatelessWidget| A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |A menu in a restaurant|nothing in this app changes|
|StatefilWidget| A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |A sign in a wall, like a Wi-Fi Password|home.dart, Navigator.|
|Navigator| Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |A social services person that halps people navegate trough the goverment programs|home.dart, Navigator.pushNamed(context, '/background')|
|Padding| Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |Any protection material that is used between the objects|background.dart, Padding( padding: const EdgeInsets.only(left: 100.0)|
|Center| Aligns content in the center of the screen or container. | `Center(child: ...)` |A red dot in a gun sight|home.dart, body: Center(, etc|
|Wrap| Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |Whan you move an object form one box to another|background.dart, Wrap( alignment: WrapAlignment.center, children:|
|@override| This marks a method as one that’s replacing a method in a parent class. | `@override` |When someone changes his hair style|in alt_design_screen.dart, @override, Widget build(BuildContext context)|
|WidgetBuild| The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |When you use the instuctions yo build a lego |in alt_design_screen.dart, Widget build(BuildContext context) { final List<Map<String, String>> dogInfo = [|
|build()| Required in every widget class to describe what to show. | `build` |Any instructions of how to build something|in alt_design_screen.dart, build(BuildContext context|
|BuildContext| A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |your specific office in a big building|in alt_design_screen.dart, (BuildContext context) { final List<Map<String, String>> dogInfo = [  |
|Super.key| A keyword used to pass a value to the parent widget. | `super.key` |A music streaming application|in Info.Card, super.key, required this.imageUrl, required this.description,|
|Const| A keyword that means the value won't change and is set once. | `const` |values that never change like Pi|in Info.Card,  margin: const EdgeInsets.symmetric(vertical: 8, horizontal: 16), padding: const EdgeInsets.all(12),|

---

### Code Definitions


| Term | Definition                        | Base Structure / Syntax  | Real Life Example | App Example |
|------|-----------------------------------|--------------------------|-------------------|-------------|
|Variable| A named container used to store a value that may change.     | `var x = 5;` |A person's age|main.dart, string title: 'TSA Portfolio',|
|Constant| A fixed value that cannot change once set.                   | `const PI = 3.14;`|A answer in a online test|main.dart, const MyPortfolioApp({super.key})|
|Data type| The kind of value a variable holds, like numbers or text.    | `int`, `String`, `bool` |price on a store or texting on your phone|home.dart, Text|
|String| A sequence of characters used to represent words or text. | `"Hello World"` |Texting| home.dart, Text 'HI, How are you?',|
|Integer| Whole number values. | `int age = 16;` |number of objects in a box|home.dart, const SizedBox(height: 20),|
|Double| Number values with decimals. | `double age = 16.2;` |buy products in a store|background.dart, padding: const EdgeInsets.only(left: 100.0),|
|Boolean| A value that can be true or false. | `bool isLoggedIn = false;` |The light are on or off|  |
|List| A collection of values in a specific order. | `List<String> names = [];` |The list of the name of the students|  |
|Null| A special value that means “nothing.” | `String? name = null;` |When you don't have the name of a contanct|  |
|Function| A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |The tax added to each type of thing you buy|  |
|Parameter| The information passed into a function to change how it works. | `greet(String name)` |The amout of money you put into the bank|  |
|Return| The result a function gives back. | `return total;` |a vending machine|  |
|Scope| Where a variable or function can be used. | (No set syntax — concept-based) |when you can bild thing or not in your house|  |
|Class| Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |the thing that the students need to do|  |
|Object| A specific version of a class. | `Dog myDog = Dog();` |the student|  |
|Property| A variable that belongs to a class/object. | `String name;` |a student's backpack|  |
|Method| A function that belongs to a class. | `void bark() {}` |whare a student is going|  |
|Constructor| A special function used to set up a class when it’s created. | `Dog(this.name);` |How whe crate a cookie|  |
|Abstraction| Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |when you clik on the space bar|  |
|Override| Changing how a built-in or inherited function behaves. | `@override` |When you overwrite something like your speed|  |
|Void| A function that does not return a value. | `void printMessage() {}` |When you change your name|  |
|          |          |         |           |         |
|          |          |         |           |         |
|Scanner| Creates a scanner object to take input from user | Scanner in = new Scanner(System.in);|           |         |
|Import Scanner| Gives access to Scanner class, requires at top | import java.until.Scanner; |           |         |
|Print line statement| prints the contnt in the parenthesis, adds lie after | System.out.print(" "); |           |         |
|Print statement| prints the content in the parethesis, adds line after | System.out.print(" ") |           |         |
|Input nextLine| reads in a String from the user | reads in a String from the user |  input.nextLine();|         |
|Input nextInt| Reads in an int from the user | input.nextInt(); |           |         |
|Input nextDouble| Reads in a double (decimal) from the user | input.nextDouble(); |           |         |
|Input nextBoolean| Reads in boolean (true/false form the user | input.necxtBoolean |           |         |
|Arithmetic operators|  + - * / % (modulid, return the remainder from dividing)  |     |           |         |
|Compound operators| applies the result to the variable | += -= *= %= ++(adds 1)|           |         |
|Maximum int| The max value an int can hold: 2147483647 | Integer.MAX_VALUE |           |         |
|Minimum int| The minimum value an int can hold: -2147483648 | Integer.MIN_VALUE |           |         |
|Integer overflow| Int MAX_VALUE + 1 == MIN_VALUE, it wraps around  a |         |           |         |
|integer uderflow| When the resul is below MIN_VALUE |         |           |         |
|Round-off error| an approx. of the actual value, result is rounded to the nearest value that fits within the available bits |         |           |         |
|Overloaded method/function or contructor| USes the same name, but has different parameters | Pizza(), Pizza(String toppings) 2 contructors, first is a default cheese pizza, 2nd has 1 topping |           |         |
|Algorithms| Define step by step processes to follow when completing a task or solving a problem | no syntax | Make a grilled cheese | Verify user |
|Sequencing| Define an order for when steps in an algorithm are completed | Follows 1, 2, 3 | which step comes first in making a grilled cheese | Get bread, add butter, add cheese |
|index| location value of each character im a String or list, starting at 0 | "Hello" index of 'e' is 1 |         |
|          |          |         |           |         |
|          |          |         |           |         |
|          |          |         |           |         |
---






-[Notebook Style Guide](#-Style-Guide-for-Coding-Notebooks)

##  Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:

# My Coding Notebook
## Day 1
### Notes
### Practice
🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

✅ Example:


**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print
💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.
✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```
🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:


1. Define the class
2. Write the main method
3. Test your program

- Variables
- Loops
- Conditionals
✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:


- [x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning
➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:


> 💡 Remember: Loops repeat code until a condition is false.
📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:


| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |
🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:


[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![ Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/-mark.svg)
📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:


<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

bash

</details>
📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:


This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.
🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.


