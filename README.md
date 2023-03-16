# Lab-5_202001136
## IT314-Software Engineering Lab-5 Static Analysis

#### Static Analysis:
Static analysis is a method of examining the source code of a software program without
executing it. Static analysis can help detect errors, bugs, vulnerabilities, and other quality issues
in the code. Static analysis tools can perform various tasks such as checking syntax, style,
logic, data flow, control flow, and security. Static analysis can improve the reliability,
performance, and maintainability of software by identifying and correcting defects early in the
development process.
#### Static Analysis Tools:
Static analysis tools are software tools that analyze the source code of a program without
executing it. They can help developers find and fix errors, bugs, vulnerabilities, code smells, and
other quality issues in their code. Static analysis tools can also measure various metrics of the
code, such as complexity, readability, maintainability, test coverage, and documentation. Static
analysis tools can be integrated into the development process as part of the code editor, the
version control system, or the continuous integration pipeline. Some examples of static analysis
tools are SonarQube, PMD, ESLint, and Pylint.
#### List of tools:
##### Python:
* Mypy
* Pylint
* Pyflakes
* Pycodestyle (pep8)
* Flake8
* Prospector
* Bandit

##### Java:
* FindBugs
* PMD
* Checkstyle
* Error Prone
* Spoon
* Spotbugs

#### Select the tool of your choice. Select a git repository, use the selected tool and analyze the files from the selected repository. Submit the tool output and understanding of the errors.

Here, I am selecting the Git repository folder - https://github.com/TheAlgorithms/Python/tree/master/data_structures/heap
and I am using Pylint for static analysis.

##### Running Static Analysis for the Python file binomial_heap.py gives the following output: 

![image](https://user-images.githubusercontent.com/104089036/225572187-f9d4d71c-8f4d-4aa8-bd0e-9025c66cfbb2.png)

The first error recommends to reomve the else statement and de-indent the code beacuse if the condition mentioned in the it statement is satisfied, the flow of execution will never reach the end of the function as the return statement is at the end of the if block. So, the else statement is unnecessary and can be removed. The code where the error occurred is shown below:
![image](https://user-images.githubusercontent.com/104089036/225575437-765da03b-9cdb-4b7c-8f02-e225580c7a19.png)

The second error indicates that the class should have a few methods to operate on the data that they hold as Pylint considers that classes are not meant to just store data. 
The third and fifth errors indicate that there are too many branches in a function or method which makes it tedious to follow.
The fourth error indicates that there is an absence of docstrings after the definition of the function, class, module or method. A docstring is a string literal that is present after definition of a function, class, module or method.

#### Running Static Analysis for the Python file heap_generic.py gives the following output: 

![image](https://user-images.githubusercontent.com/104089036/225579134-039a090b-bedf-411b-8827-abc811ef4661.png)

The first error indicates that there is an absence of docstrings after the definition of the function, class, module or method. The second error is displayed when there is a reference to an object that initialized as a non-subscriptable object. The code where the second error occurs is given below:

![image](https://user-images.githubusercontent.com/104089036/225580267-67722f71-b173-4f3c-8084-a46101a5afa5.png)

#### Running Static Analysis for the Python file heap.py gives the following output: 

![image](https://user-images.githubusercontent.com/104089036/225580932-9516c7e2-72f5-401a-bd80-d5c2acd90676.png)

The first and fifth errors indicate that there is an absence of docstrings after the definition of the function, class, module or method. The second and fourth errors are displayed when the name doesn’t conform to naming conventions associated to its type (constant, variable, class...). The code where the second and fourth errors occur are given below:

![image](https://user-images.githubusercontent.com/104089036/225582921-8cd7cc84-e79b-4608-b45d-2bb6a6c7d422.png)

![image](https://user-images.githubusercontent.com/104089036/225583179-36add999-6501-44d0-82e3-81220bf07852.png)

#### Running Static Analysis for the Python file max_heap.py gives the following output:

![image](https://user-images.githubusercontent.com/104089036/225583379-c427680e-44a3-4753-9c20-fe3f4a8ccb4c.png)

Here, both the errors are caused due to the absence of a docstring. The code where the first and second errors occur are given below:

![image](https://user-images.githubusercontent.com/104089036/225583652-bb4c6229-e408-4b7a-9556-22a224d25382.png)

![image](https://user-images.githubusercontent.com/104089036/225583893-82ebe667-9fd4-4bea-9420-93f353742858.png)

#### Running Static Analysis for the Python file min_heap.py gives the following output:

![image](https://user-images.githubusercontent.com/104089036/225584138-c2877847-b334-480c-aef4-c640c922b5a3.png)

Here, most of the errors are shown because of the absence of the docstring. The other error W0621 is shown when a variable’s name hides another variable name defined in the outer scope. The C0103 errors are displayed when the name doesn’t conform to naming conventions associated to its type (constant, variable, class...).

#### Running Static Analysis for the Python file randomized_heap.py gives the following output:

![image](https://user-images.githubusercontent.com/104089036/225585146-aa9ed7e8-00ad-46b5-aaef-07cc98c49bec.png)

Here, the error caused is due to the absence of a docstring. The code where the error occurs is given below: 

![image](https://user-images.githubusercontent.com/104089036/225585585-afe5818d-6f65-44d3-b364-b1fc10baedd5.png)

#### Running Static Analysis for the Python file skew_heap.py gives the following output:

![image](https://user-images.githubusercontent.com/104089036/225585807-bc0d1a42-4856-4c57-8a74-4dcedbd0a09e.png)

Here, the error caused is due to the absence of a docstring. The code where the error occurs is given below: 

![image](https://user-images.githubusercontent.com/104089036/225585585-afe5818d-6f65-44d3-b364-b1fc10baedd5.png)
