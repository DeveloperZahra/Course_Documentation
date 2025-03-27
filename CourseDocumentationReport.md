## 1. **_Software Development Life Cycle ( SDLC ):_**
Software development life cycle (SDLC) is a structured process that is used to design, develop, and test good-quality software.
SDLC, or software development life cycle, is a methodology that defines the entire procedure of software development step-by-step. 
The goal of the SDLC life cycle model is to deliver high-quality, maintainable software that meets the user’s requirements.
>* _**There are 6 faces for SDLC:**_
1. **analysis** 
2. **design** 
3. **developme0nt** 
4. **testing** 
5. **deployment** 
6. **maintenance**

>* _**There are several functions that fall under it:**_

1. **__Users:__** in Entire Operations, a user ID can be used to enter the system. Several users can log on to Entire Operations with the same user ID and password at the same time. 
For reasons of data security and in order to trace data modifications, however, each user usually has a personal user ID and password. 
User roles are crucial for protecting sensitive information from unauthorized access. By assigning the appropriate roles and permissions, businesses can control who can view, edit, modify, or delete data.
This granular level of control helps maintain data integrity and accuracy.
2. **__Tester:__** evaluating and updating software to ensure it remains functional, secure, and efficient, even after changes or updates.
The role of tester is to validate the system's features, capabilities, and interactions with different components.
3. **__Support managers:__** is a professional responsible for overseeing the maintenance operations of a facility or organization.
They are responsible for ensuring that all maintenance activities are completed in a timely and efficient
The role of support managers is manage and lead a team of customer support representatives, providing guidance, training and performance evaluation to ensure high quality service.
Also supervises the team that interacts directly with customers and follows up on complaints, inquiries and all customer service related matters.

![image](https://media.geeksforgeeks.org/wp-content/uploads/20230127172040/Best-SDLC-Methodologies.jpg)
--------------------------------------------
## **__2. Agile Methodology and Scrum framework:__**
* _**Agile:**_ An integrated process that works non-stop and complements each other and is continuous in developing products and releasing new products, allowing for segmentation as it is subject to change with the start of priority.
It is considered more flexible to improve and reprioritize product backlogs so that it always delivers high quality products.
Agile methodology is characterized by its iterative and flexible approach to software development.
It emphasizes collaboration among cross-functional teams and prioritizes adaptability to changing requirements throughout the development process.
* _**Scrum:**__ is a management framework that teams use to self-organize and work towards a common goal.
also  agile project management framework that helps teams structure and manage their work through a set of values, principles, and practices.

![image](https://www.notifyvisitors.com/pb/wp-content/uploads/2020/12/agile-vs-scrum-banner-1024x341-2-1.webp)
________________________________________________
## **__3.Git Version Control:__**

Git is a distributed version control system, meaning that it allows developers to work on their own local copies of a project
Git helps manage and track changes to code, but it does so in a decentralized way
This design makes Git fast, scalable, and highly resilient to issues like server failures

>* _**Key Features of Git:**__
1. **_Version Tracking:_** Git follows all adjustments done in one record, letting you revert to old releases without trouble.
2. **_Collaboration:_** Different programmers can work on a similar task at the same time without clash.
Branching: You have the option to create distinct branches for new attributes, bug repairs or tests.
3. *__Distributed System:__* Every programmer has an entire version of the project implying that it is decentralized software.
Log of Commits: With this feature, Git maintains an account of all commit actions (changes), 
which makes understanding how a project has evolved over time much easier.

![image](https://homes.cs.washington.edu/~mernst/advice/version-control-ops-local-vs-remote.svg)

!{image}(https://files.slack.com/files-pri/T08EFTFHWSK-F08GDK24NBA/git_commands2.png)

>* **_There four main stages in using git as the following:_**

1. **__Working Directory:__** It’s the workspace where the code can be modified and change without any restrictions.

2. 	*__Staging Area:__* It’s the space where the codes are reviewed before saving them as a new copy of the project and also here no modification can be made to the written code.
3. *__Local repo:__* It’s the space where the codes are saved as a new copy of the project and be ready to push to the remote repo.
4. *__Remote Repo:__* It’s a remote space where the main project is stored so that all team members can share their work with the rest of the team and get the latest update from the project.

>⦁ **THE CLOUD REPOSITORIES THAT USE GIT VERSION CONTROL:**

![image](https://lh4.googleusercontent.com/-MgrAPEm_n7eH-Ejcptx4n6YD2CAb8rdIfjJnRL7vhGK6ik8FdKRoXw_QNzWyB5KOoXS_1J9fHoCQVDQvIj62FFII-7m8IkNFDLNwV7QAR9UdcycdpsmtWvSBWyKjzvhnJ1lSBg0)

Features|	Bitbucket |	GitHub 	|Gitlab
--------|-------------|---------|------
Free private repositories|	Yes	|Yes	|Yes
Free public repositories|	Yes|	Yes|	Yes
Merge Request/Issue Templates|	No| 	Yes|	Yes 
Integrated CI|	yes|	No| 	Yes
Open-source|No|	No| 	Yes 
File storage|	Yes|	Yes|	Yes
Integrations|	Yes|	Yes|	Yes
Analytics	|Yes |	No | 	Yes


------------------------------------------------------
## **__4. Algorithm design ( Pseudo code and flowchart ):__**
An algorithm is more general and is a step-by-step process based on specific and organized instructions that takes inputs, processes them, and then produces outputs.
One of the most important characteristics that an algorithm must have is that it is correct, clear, and has an end.
An algorithm is a step-by-step procedure to solve a problem or perform a task.

> *  _**Characteristics of a Good Algorithm:**_

1. **__Correctness:__** It should solve the problem correctly.
2. **__Efficiency:__**  It should run in a reasonable amount of time.
3. **__Clarity:__**  Easy to understand and implement.
4. **__Finiteness:__** It must have an end.
5. **__Generality:__** It should work for multiple inputs. 

> * _**Algorithms are solved using:**_
 
1. pseudocode 
2. flowchart 
3. programming language


> * _**Types of Algorithms:**_

1. Sequential Algorithm (Step-by-step Execution)
2. Iterative Algorithm (Using Loops)
3. Recursive Algorithm (Function Calls Itself)

> * _**Algorithm Components:**_

1. *__Variables:__* used to store values
2. *__Input and Output statements:__* used to get and display data
3. *__Conditional Statements (Decision Making):__* used to make Decision
4. *__Loops (Iteration):__* used to repetition
5. **__Functions (Procedures):__** used to code reuse
6. *__Arrays and Lists:__* used to store many values in same variable

>* __**reverse a string:(PesudoCode)**__

1. start 
2. display "Reverse the string"
3. display "enter the string to reverse it"
4. prompt user for za
5. read za
6. for (X=0 to (za[x] not=to null))step x=x+1
7. end for 
8. display "reverse of the string is"
9. for((x=x-1 to (x>=()) step i=i+1
10. display za[x]
11. end for
12. end 
	
* **__FlowChart__**

![image](https://media.geeksforgeeks.org/wp-content/uploads/flowchart-to-find-reverse-of-a-number.jpg)
-------------------------------------------------------
## **__5. Web Development Stacks:__**

A web development stack is a combination of tools and technologies 
used to create websites or web applications

>* *__Full stack .Net web development course components and tools:__*
	
!{image}(https://files.slack.com/files-pri/T08EFTFHWSK-F08F1Q6UZML/img_5748.jpg)

![image](https://cdn.educba.com/academy/wp-content/uploads/2019/09/Fornt-End-VS-Back-End.png)

Full stack development is the process of developing both the frontend and backend of 
applications. Any application has a frontend (user-facing) component and a backend 
(database and logic) component. The frontend contains the user interface and code 
related to user interactions with the application. The backend contains all the code 
required for the application to run, including integrations with data systems, communicating with other
applications, and processing data.

------------------------------------------------
## *__6. Programming Paradigms:__*
![image](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*sH3laAdBV74SCHWGRzjVIg.jpeg)

A programming paradigm is a fundamental approach or style of programming that provides
a set of principles, concepts, and techniques for designing and implementing computer
programs. It defines the structure, organization, and flow of the code, as well as the
methodologies for problem-solving and expressing computations.

>* _**Here are to some popular programming paradigms:**_
	
	1. Procedural Programming
	2. Object-Oriented Programming (OOP)
	3. Functional Programming (FP)
	4. Declarative Programming
	5. Event-Driven Programming
	6. Concurrent Programming


![image](https://www.computersciencedegreehub.com/wp-content/uploads/2021/03/Brief-History-of-Programming-Languages.jpg)

-------------------------------------------------
## *__7. Algorithm programming components:__*
10 important items that should be in the algorithm are listed. These features that should be in 
the algorithm; Clarity, Input, Output, Accuracy, Efficiency, Configuration, 
Processing Time, Memory Usage, Splitting into subproblems, Reusability.

   1.*__Clarity:__* The algorithm should state the steps to be performed step by step in a clear and understandable way.

   2. *__Input:__* The algorithm must specify what type of data to use as input and how to get that data.
   3. *__Output:__* The algorithm must specify what kind of output will be obtained as a result of the operation and how this output will be presented.
   4.* __Accuracy:__* The algorithm must fully and accurately describe the operations required to produce the correct results.
   5. *__Efficiency:__* The working of the algorithm should be designed to solve the given problem as soon as possible.
   6. *__Configuration:__* The algorithm should have a structure that follows step-by-step processes from a starting point.
   7. *__Processing time:__* The algorithm must specify how much time is needed to process the given inputs.
   8. *__Memory usage:__* The algorithm must specify how much memory the data will use and whether this memory usage is sufficient.
   9. *__Splitting into subproblems:__* The algorithm should make large problems easier to solve by dividing them into smaller subproblems.
   10. *__Reusability:__* The algorithm should be reusable for similar problems.

   ![image](https://miro.medium.com/v2/resize:fit:640/format:webp/0*H_GPo7_245Uivk77.gif)
   -------------------------------------------------
   ## _*8.Types of programming languages ( based on machine interaction, execution )*_
   > *__1.  Procedural programming languages:__*
	
A procedural language follows a sequence of statements or commands in order to achieve a desired output. Each series of steps is called
a procedure, and a program written in one of these languages will have one or more procedures within it. 
Common examples of procedural languages include:
       
	   *C and C++        *Java
	   *Pascal           *BASIC 

> *__2. Functional programming languages__* 

Rather than focusing on the execution of statements, functional languages focus
on the output of mathematical functions and evaluations. Each function–a reusable 
module of code–performs a specific task and returns a result. 
The result will vary depending on what data you input into the function. 
Some popular functional programming languages include:

            *Scala          *Erlang
		*Haskell        * Elixir

> *_3. Front-end & back_end languages:_*

* Front-end languages are primarily concerned with the ‘user’ aspect
of the software. The front end deals with all of the text, colors, 
buttons, images, and navigation that the user will face when navigating 
your website or application. Anyone with a background in graphic design 
or art may be more inspired to begin learning one of the front-end languages. 

Some examples of front-end programming languages include:
     
	 *HTML           *CSS 

	 *JavaScript     *React 
* Back-end languages deal with storage and manipulation of the server 
 side of software. This is the part of the software that the user does
 not directly come into contact with but supports their experience behind 
 the scenes. This includes data architecture, scripting, and communication
 between applications and underlying databases. 
 Anyone with experience in mathematics or engineering may
find more interest in back-end development.

Some examples of back-end programming languages include:

         *JavaScript   *PHP
	     *Java         *Python
	     *Ruby         *C#

----------------------------------
## _*9. Comparison of compiler and interpreter:*_

Interpreter| Compiler
-----------|-----------
Translates program one statement at a time.| Scans the entire program and translates it as a whole into machine code.
Interpreters usually take less amount of time to analyze the source code. However, the overall execution time is comparatively slower than compilers.| Compilers usually take a large amount of time to analyze the source code. However, the overall execution time is comparatively faster than interpreters.
No Object Code is generated, hence are memory efficient.| Generates Object Code which further requires linking, hence requires more memory.
Programming languages like JavaScript, Python, Ruby use interpreters.| Programming languages like C, C++, Java use compilers.

> * Working of Compiler and Interpreter
	
![image](https://cdn.programiz.com/sites/tutorial2program/files/compiler-interpreter-working.png)

























	













