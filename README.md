# Introduction

This document serves as a comprehensive guide outlining the coding style conventions that students and academic staff are encouraged to adhere to. Code style is a set of rules or guidelines that governs the layout of source code. These rules dictate how code should be formatted, structured, and written to ensure consistency, readability, and maintainability across a codebase. Additionally, this guide provides insight into the rubric used for evaluating coding tasks, ensuring alignment with industry standards and best practices.

## Purpose

This document aims to provide a guide to coding style, offering guidance, references, and criteria for evaluating adherence to industry standard coding conventions.

## Objectives:

- Establish and maintain uniform coding styles across various bootcamps.
- Ensure that code produced by students meets industry standards for readability, consistency, and maintainability.
- Provide students with reputable style guides to enhance their understanding and application of coding style principles.
- Assess students adherence to coding style guidelines and provide constructive feedback for improvement.

# Prescribed Style Guides:

## Python
# Python PEP 8 Style Guide: A Beginner's Cheat Sheet 🐍

## What is PEP 8?
PEP 8 is like a style manual for Python code. Think of it as the "grammar and etiquette" guide for writing clean, readable Python programs. Following these rules helps make your code look professional and easy for other programmers to understand.

## Indentation
- Python uses indentation to define code blocks, so it's crucial for avoiding errors.
- Use **4 spaces** per level of indentation to ensure consistency.
- **Never mix tabs and spaces** to prevent IndentationError.
 
 Example:
  ```python
  def my_function():
      if True:
          print("Properly indented!")  # 4 spaces in
  ```

## Line Length
- Limit lines to **79 characters** for code and **72 characters** for comments to improve readability.
- If a line is too long, break it into smaller parts for clarity and better organization.
- Use parentheses to wrap long expressions when splitting lines.
 
 Example:
  ```python
  # Good: Use parentheses to break long lines
  long_variable = (first_part + 
                   second_part + 
                   third_part)
  ```

## Naming Conventions

### Variables and Functions
- Use **lowercase** with **underscores** to improve readability and follow Python’s naming standard.
- Choose **clear** and **descriptive** names to make the purpose of the variable or function easy to understand.
 
 Example
  ```python
  # Good ✅
  user_name = "Alice"
  calculate_average_score()

  # Avoid ❌
  userName = "Bob"
  calcAvgScore()
  ```

### Classes
- Use **CamelCase** for class names to distinguish them from variables and functions.
- Always start class names with a capital letter to follow standard Python naming conventions. 
 
 Example:
  ```python
  class StudentRecord:
      def __init__(self, name):
          self.student_name = name
  ```

### Constants
- Use **ALL_UPPERCASE** with underscores for constants to clearly indicate that their values should not be changed. This helps differentiate them from regular variables.
 
 Example:
  ```python
  MAX_STUDENTS = 30
  PI_VALUE = 3.14159
  ```

## Whitespace
- Use blank lines to separate functions and logical sections of your code, making it easier to read.
- Avoid extra spaces inside parentheses or before commas to maintain consistent formatting and prevent unnecessary clutter.
 
 Example:
  ```python
  # Good spacing
  def function_one():
      pass

  def function_two():
      x = (1, 2, 3)  # No space inside parentheses
      list_of_items = [1, 2, 3]  # No space before comma
  ```

## Comments and Docstrings
- Use comments to explain *why* something is done, not *what* is done, as the code itself should already be clear on what it's doing.
- Write clear and concise docstrings for functions to explain their purpose, parameters, and return values.
 
 Example:
  ```python
  def calculate_grade(score):
      """
      Converts a numeric score to a letter grade.
      
      Args:
          score (int): Numeric score between 0-100
      Returns:
          str: Letter grade (A, B, C, etc.)
      """
      # Complex grade calculation logic
      if score >= 90:
          return 'A'
      # More grade ranges...
  ```

## Imports
- Always place imports at the top of the file, before any code, to keep your dependencies organized.
- Organize imports by category: first, standard library imports; then third-party imports; and finally, local module imports. This improves clarity and ensures a logical structure.
  
- Example:
  ```python
  # Standard library
  import math
  import random

  # Third-party
  import numpy
  import pandas

  # Your own modules
  import my_custom_module
  ```

## Best Practices for Clean Code
- Consistency is key for writing clean, maintainable code.
- Use tools like `Flake8`, `pylint` or `black` to assist in maintaining style consistency.
- Practice regularly to improve your coding skills and reinforce good habits.

## Why PEP 8 Matters
PEP 8 isn't about striving for perfection, but rather ensuring your code is:
- Easy to read, so others (and your future self) can quickly understand it.
- Easy to understand, allowing anyone to follow your logic and intentions.
- Easy to maintain, making it simpler to modify, update, and debug in the future.

## Additional Resources
- [PEP 8 – Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
- [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)

Happy Pythoning! 🐍✨

## SQL

- [SQL Style Guide](https://www.sqlstyle.guide/)

## JavaScript

- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

## HTML/CSS

- [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)

## Java

- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)

## PHP

- [PHP Extended Coding Style](https://www.php-fig.org/psr/psr-12/)
- [PHP Standards Recommendations](https://www.php-fig.org/psr/)

## Bash

- [Bash Style Guide](https://google.github.io/styleguide/shellguide.html) 

# Code style extensions

## Python
The [Flake 8](https://marketplace.visualstudio.com/items?itemName=ms-python.flake8) extension is a linting tool for Python code. Flake8 makes it convenient to check code for common errors such as syntax errors. It also helps to enforce some of the coding standards and best practices from the PEP 8 Style Guide regarding indentations, whitespaces, and more.  

### Installation
1. Open VS Code and click on the extension's icon on the left panel.
2. Search for Flake8 in the search bar.
3. Click on the "Flake8" extension by Microsoft and then the install button.

![Flake8](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/959fe0c2-55fe-4179-84aa-90aa59ae9869)

## JavaScript, HTML and CSS
[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) is a code formatting tool that automatically formats code when saved, according to a set of predefined rules and conventions. This extension supports JavaScript, HTML and CSS, but it doesn't support Python. However, please note that Prettier focuses solely on code formatting and does not perform linting or provide warnings about violations of coding style guidelines as Flake8 does. 

### Installation
1. Open VS Code and click on the extension's icon on the left panel.
2. Search for "Prettier" in the search bar.
3. Click on the "Prettier - Code formatter" extension by Prettier and then the install button.

![Prettier](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/e0656b41-569a-4309-bead-86a61b2fe063)

### Settings
After installation, you'll need to adjust the settings to enable Prettier. You may follow these steps:

1. Click on the "manage" icon and then "extension settings".
![Prettier step 1](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/775ee0f4-03a4-427f-baf7-99e0d76580d3)

2. Type "default" in the search box and navigate to the "Text Editor" folder. Next, set Prettier as the default formatter from the dropdown menu. 
![Prettier step 2](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/e10ea9ee-e2f0-4ec4-87bd-76872edb4229)

3. Lastly, type "format" in the search box and navigate to "Text Editor > Formatting". Check the boxes to format the file on paste, save and type.
![Prettier step 3](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/9022f993-3368-4c1a-a8fe-c02190ee3db5)

## Note
While the above mentioned tools can provide helpful suggestions for maintaining coding style, it's important to note that they should be used as guidance. Adherence to the recommended style guides specified in this document takes precedence over the suggestions provided by these tools. Ultimately, it's the responsibility of students and all academic staff to ensure that the code aligns with the coding conventions outlined in the recommended style guides.

## Implementation and Evaluation

### Grading rubric:

The rubric that is used for grading HyperionDev students follows a grading scale of 1 - 4 and includes four metrics. One of these metrics is coding style which assesses various aspects such as indentation, spacing, naming conventions, commenting practices, and overall code organization.

![Asynchronous review rubric](https://github.com/HyperionDevBootcamps/HyperionDev_Style_Guides/assets/167426222/69377e77-6c97-459b-954b-e4fc3701a832)

## Student Implementation:

To ensure adherence to coding style guidelines, students are encouraged to:

- Familiarize themselves with the recommended style guides specific to the bootcamp they are enrolled in.
- Implement the specified coding styles in their tasks.
- Reference the style guides for guidance and clarification on coding conventions.
- Take responsibility to strive for consistency, readability, and maintainability in their codebase.

## Mentor Evaluation:

Mentors offer feedback and guidance to foster growth and development in the student’s coding journey. They are therefore responsible for:

- Reviewing students' code submissions with a focus on adherence to the recommended style guides.
- Providing constructive feedback on coding style by referencing specific sections of the style guides.
- Guiding students in understanding and implementing coding conventions.
- Supporting students by reinforcing good coding habits that align with industry standards and best practices.

## Resolving Conflicts:

Different style guides might offer conflicting guidance on coding conventions.
Therefore, we have compiled the aforementioned list of reputable style guides for your benefit.
These guides are helpful for understanding coding conventions and should be prioritized for the assignments.
In the event of discrepancies between these guides and the one utilized, it will be imperative to explicitly specify the guide being adhered to in order to resolve any conflicts.

## Revision and Maintenance:

To adapt to evolving industry practices, continuous improvement of coding standards is reflected in these guides. Therefore, this is a living document that undergoes periodic revision and maintenance to ensure its relevance.
