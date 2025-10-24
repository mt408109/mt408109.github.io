## My Coding Notebook

## Table of Contents
- [Fultter Notes](#flutter-notes)
  - [What is Flutter?](#what-is-flutter)
  - [Key Terms and Definitions](#key-terms-and-definitions)
  - [Layout and Design Widgets](#layout-and-design-widgets)  
  -  [Definitions with Structures](#flutter-definitions-with-structures)
- [Code Definitions](#code-definitions)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

## Flutter Notes

### What is Flutter?
- Definition:
- Why is it useful?

---

### Key Terms and Definitions

## Flutter Definitions with structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|Main()      | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |Starting car, clicking app on phone  |main.dart,void main() => runApp(MyPortfolioApp());  |
|MaterialApp      | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  |main.dart return MaterialApp( debugShowCheckedModeBanner: false, title: 'TSA Portfolio',theme: ThemeData(  |
|Scaffold      | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |Notes, worksheets, job application  |showcase.dart,return Scaffold( body: Column (mainAxisAlignment: MainAxisAlignment.start, children: [
|Column      | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |term  |showcase.dart, Column( children: [  |
|Row      | A widget that shows things side-by-side. | `Row(...)` |related to that term, stack of rows, posters  |InfoCard.dart, child: Row( children: [   |
|Container      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |changing background  |InfoCard.dart, return Container(   |
|Text      | A widget to display text on the screen. | `Text('Hello')` |on a app, title of app  |InfoCard.dart,  child: Text( description, style: const TextStyle(color: Colors.white),  |
|Image.network      | A widget to show an image using a link from the internet. | `Image.network('https://...')` |  |InfoCard.dart, child: Image.network(imageUrl, width: 100, height: 100, fit: BoxFit.cover), ),  |
|ElevatedButton      | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |send to profile  |showcase.dart Wrap(alignment: WrapAlignment.center, children: puppyUrls.map((url) => puppyImage(url)).toList()),ElevatedButton(  |
|onPressed      | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |change the font, change the document  |showcase.dart onPressed: () => Navigator.pushNamed(context, '/alt'),|
|StatelessWidget      | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |about page  |showcase.dart class InfoCard extends StatelessWidget { final String imageUrl;  | 
|StatefulWidget      | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |locations, background chnages color  |alt_design_screen.dart class AltDesignScreen extends StatelessWidget { |
|Navigator      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  |home.dart Navigator.pushNamed(context, '/background'), child: const Text('Next'),  |
|Padding      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |Make space  |InfoCard.dart padding: const EdgeInsets.all(12), decoration: BoxDecoration(  |
|Center      | Aligns content in the center of the screen or container. | `Center(child: ...)` |Welcome in the center in a page  |home.dart return Scaffold( body: Center( child: Column(  |
|Wrap      | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |  |showcase.dart Wrap(alignment: WrapAlignment.center, children: puppyUrls.map((url) => puppyImage(url)).toList()),  |
|@override      | This marks a method as one that’s replacing a method in a parent class. | `@override` |app build, customize, individual  |InfoCard.dart @override Widget build(BuildContext context) {  |
|Widget build      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |Define screen |Widget build(BuildContext context) {return Scaffold( |
|Build()      | Required in every widget class to describe what to show. | `build` |canva, Pdf  |background.dart  Widget build(BuildContext context) {  |
|BuildConext      | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |background.dart  Widget build(BuildContext context) { return Scaffold(  |
|super.key      | A keyword used to pass a value to the parent widget. | `super.key` |emailing teacher  |alt_design_screen.dart const AltDesignScreen({super.key});  |
|Const      | A keyword that means the value won't change and is set once. | `const` |settings,title of app  |InfoCard.dart const SizedBox(width: 12), Expanded( child: Text(  |

## Code Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building block of a Flutter app. Everything. is a widget                      | Test,image,containers,column                                          |
| MaterialApp      | The root of the app. Sets up routes and the theme. | Found in main.dart                                          |
| Scaffold         | Provides basic visual layout - like a header, body, floating button                                                 | Each screen uses it                                          |
| StatelessWidget  | A widget that doesnt change                      | Most of the screen files                                          |
| StatefulWidget   | A widget that can change over time                                                 | Used in MyHomePages()                                           |
| Navigator        | Manages screen transitions                       | Navigator.pushNamed(context, '/page2');                                          |
| AppBar           | Top navigation bar                               | title of each page appears here                                          |
| Column           | Vertical layout                                  |                                           |
| Row              | Horizontal layout                                |                                           |
| Container        | Wraps content with padding, margin, or color     |                                           |
| Text             | Display test                                     |                                           |
| Image.network    | Displays imagines from a URL                     |                                           |
| Padding          | Adds space around a widget                       |                                           |
| Center           | Center its child                                 |                                           |
| Main()           | The function that runs the app                                | Found in main.dart                                          |
| Name routes           | Predefined paths to navigate between screens                                 | '/','/page2','/page3',etc.                                          |
---

### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|Variable | A named container used to store a value that may change. | `var x = 5;` |Goals in soccer, score  |in main.dart, title: 'TSA Portfolio',  |
|Constant | A fixed value that cannot change once set. | `const PI = 3.14;` |Username, files, profile imgaine,text, carpet  |main.dart,const MyPortfolioApp({super.key});  |
|Data type      | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool`|Video, images, Video games |main.dart, bool, debugShowCheckedModeBanner: false,  |
|String      | A sequence of characters used to represent words or text. | `"Hello World"` |Title on apps, Game mode, messages, store username  |InfoCard.dart final String imageUrl;  |
|Integer      | Whole number values. | `int age = 16;` |Streak, age, clocks  |  |
|Double      | Number values with decimals. | `double age = 16.2;` |Smooth movement, calulations  |  |
|Boolean      | A value that can be true or false. | `bool isLoggedIn = false;` |If u want to open the door, Opening a app,  |  |
|List      | A collection of values in a specific order. | `List<String> names = [];` |Cards in a wallet, contact list,list of videos you like   |  |
|Null      | A special value that means “nothing.” | `String? name = null;` |username  |  |
|Function      | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |One switch for all lights, Starting car, videogame character  |  |
|Parameter      | The information passed into a function to change how it works. | `greet(String name)` |Money into bank, grocery store, passward  |  |
|Return      | The result a function gives back. | `return total;` |recipt, shipping date on a order|  |
|Scope      | Where a variable or function can be used. | (No set syntax — concept-based) |Starbucks card, smiths card, dual enrollments  |  |
|Class      | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` | what classes you take, grades in the classes, car class  |  |
|Object      | A specific version of a class. | `Dog myDog = Dog();` |student, computers,Profiles  |  |
|Property      | A variable that belongs to a class/object. | `String name;` |A airplane how many seat are in the plane, A bus what wheels or how many seats  |  |
|Method      | A function that belongs to a class. | `void bark() {}` |self driving cars, take test |  |
|Constructor      | A special function used to set up a class when it’s created. | `Dog(this.name);` |Baby certificate (name, date)  |  |
|Abstraction      | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |Driving a car without knowing the engine  |  |
|Override      | Changing how a built-in or inherited function behaves. | `@override` |super hero have different powers  |alt_design_screen.dart @override Widget build(BuildContext context) {  |
|Void      | A function that does not return a value. | `void printMessage() {}` |list of homework, marking something complete, turning on light switch not getting something in return  |  |
|scanner   |Creates a scanner object to take ipout from user |Scanner in = new Scanner(System.in); |  |  |
|import scanner |Gives access to Scanner class, required at top|import java.util.Scanner; |  |  |
|Print line Statement   | prints the content in the parenthesis, adds line after |  System.out.println(" ");  |  |  |
|input nextLine   | Reads in a string from the user  |input.nextLine(); |  |  |
|input nextInt   | Reads in an int from the user |input.nextint(); |  |  |
|input nextDouble   |Reads in a double (decimal) from the user|input.nextDouble(); |  |  |
|input nextBoolean   |reads in a boolean (true/false) from the user|input.nextBoolean(); |  |  |

[Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)
## Markdown Style Guide for Coding Notebooks

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

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
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
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

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
