## Glossary

## Algorithms

**Definition of an Algorithm.**  

An algorithm is a set of rules and instructions given to a computer that will help answer a particular problem within a number of steps. (Dutkiewicz, 1994)
One example of an algorithm is the Euclidean Algorithm otherwise known as Euclid's Algorithm, it is an algorithm used to find the Highest Common Divisor between two numbers. (Ferguson, 1999). 

 
 **Building An Application**

Several steps have to be taken in order to successfully build and implement an application.

*  One of the first steps that needs to be taken is to check the specifications which are received with a proposal from a client, what does the client require, the timescale in which the application needs to be completed in, the price the client is willing to pay etc.
* A software development life-cycle model is then chosen of which there are several types, Agile, Spiral, Waterfall and V-Model to name a few. Agile and Spiral are iterative life-cycle models, Waterfall and V-Model are sequential life-cycle models. Most programmers will already know their preferred life-cycle model, the most common type of life-cycle model used is the iterative model, clients can get the application early on in the life-cycle so they can provide feedback and any specification changes required. 
* After the specifications have been checked, the next step is to conduct a feasibility study, this isn't a feasibility study for the client (they would have already conducted one themselves) but for the building of the application itself. Is it feasible to build this program in the clients specified time and budget? After this is complete negotiations with the client can commence with final specifications being agreed upon. 
* The design can now be started, using brainstorming, flow charts, user stories and market research.
* After the design process coding can begin, using coding standards to keep code formal and readable. Comments are added to important sections of code so that in the event of a revision the programmer can easily go back and read the purpose of that block of code making it easier to change.  
* A prototype is made and sent off to the client for review, the client then can ask for amendments to be made (if amendments are not included in the contract money may be charged). This is why iterative models are so popular because of their modular nature. 
* After several prototypes have been made and a final version is agreed upon, it is implemented. (The application is released usually as Version 1.0, in some cases Open Alpha and Beta versions are released to the consumers generally as 0.X versions, the consumers essentially become part of the prototype testers giving feedback on any bugs or errors they find). 
* The final phase is maintenance, any new bugs or errors found in the code will be dealt with and to ensure the application keeps up with compatibility with new technologies that may be released. 

Here is an example of a flow chart:
![FlowChart](https://github.com/LukeFarren/TraceBall/blob/master/Flow%20Chart.png)

Here is an example of a Burn-down Graph.
![Burn-down](https://github.com/LukeFarren/TraceBall/blob/master/TraceballBurnDown.png)
## Paradigms

A programming paradigm is a model of programming based on how a program is designed, there are multiple paradigms including but not limited to Procedural, Object and Event-Driven paradigms.

 **Procedural Oriented Paradigms**

Procedural Orientated Programming (sometimes known as Imperative Programming) is generally the first paradigm a programmer is likely to encounter and use. This is linear in nature focusing on small blocks of code known as functions and subroutines that can be taken out and reused in the same application or simply added to another. (Brownlee, 2012).

Here is an example of Procedural Oriented Programming, a simple calculation program in which addition can be changed out for division, multiplication and subtraction easily.

	//Calculation Program made by Luke Farren - 2018
	#include  <iostream>
	using  namespace std;
    int main()
	    {
		    int a, b, c;
		    cout << "Please enter first number to calculate: ";
		    cin >> a; //Input integer.
		    cout << endl; // Uncessary spacing, used for asphetics.
		    cout << "Please enter second number to calculate: ";
		    cin >> b; //Input integer.
		    cout << endl;
		    c = a + b; // Change the addition sign to multiplication (*), division (/) or subtraction (-). 
		    cout <<"= " << c << endl; //Output Integer.
	    return  0;
	    }

[Link to Calculation Program](https://github.com/LukeFarren/Calculator-/blob/master/CalculatorProgramLukeFarren.cpp)

**Characteristics of Procedural Oriented Paradigms.**

* Easy to remove and reuse in additional programs.
* Focuses on small modules that act as self contained applications in their own right. 
* First paradigm a programmer is likely to use.
* Linear coding process. 

**Object-Oriented Paradigms**

Object-Oriented Programming uses entities called objects, each object has behaviours and attributes (data) that allows them to interact with other objects using message passing.  A person using Object-Oriented programming methods defines its class which encompass all relevant information required to be classed as an Object. An entity (Object) can be treated as a parent, all other objects will inherit the attributes of the parent. (Brownlee, 2012).

**Message Passing**

Message passing is a type of communication between processes mainly used in Object-Oriented Programming to send data to the other objects. (Beal, 2015)

Here is an example of Object-Oriented Programming, using JavaScript. 

	function startGame()
	{
		myGameArea.start();
		player = new component(50,50,"Green",50, 50);
		computer = new component(50,50,"Orange", 750, 550);
		myGameArea.start();
	}
[TraceBall Game Code](https://github.com/LukeFarren/TraceBall/blob/master/Game.html)

**Characteristics of Object Oriented Paradigms.**

* Has behaviours and attributes known as data.
* Can be treated as a parent.
* Uses message passing to communicate with other objects.


**Event-Driven Paradigms** 

An event-driven paradigm is written to react and respond to inputs that are either user generated or system generated, an event is an occurrence that has an effect on the system hardware or software. e.g mouse X, Y mouse movement. (Rose, n.d.).

Here is an example of Event-Driven Paradigm. 
		
	this.canvas.addEventListener("mousemove", function (m) // uses mouse input to track the mouse position.
		{
			myGameArea.x = m.offsetX;
			myGameArea.y = m.offsetY;
		}
  [Traceball Mouse Movement](https://github.com/LukeFarren/TraceBall/blob/master/Game.html)
  
  **Characteristics of Event-Driven Paradigms.**

* Uses an event listener to snoop for a specified parameter movement/s. e.g. Mouse movement.
* Can use both user inputs and system generated inputs.
* Useful in applications such as Photoshop and FPS games.
   
**Relationships between Paradigms** 

Each paradigm has its own position within a piece of code, although each paradigm is not essential in circumstances such as a simple calculation program using a Procedural-Oriented Paradigm. (Zandbergen, n.d.)

Each paradigm can be linked with one another in the following ways, Object-Oriented programming entities (objects) are a combination of different functions created using Procedural-Oriented Programming. Likewise for Event-Driven programming a function is created using Procedural-Oriented Programming to add an event listener which can detect user or system generated inputs.  

## **Debugging Process and features within an IDE**

Debugging is a process of elimination, its a method of identifying and limiting the number of bugs and glitches within a a piece of code. Unfortunately, the debugging process isn't without its own problems as eliminating one bug or error may cause other errors to appear.  (Unknown, n.d.)

The first step in the debugging process is to identify and find the error, simple spelling and punctuation mistakes are usually the first problems that are encountered, a mistake such as end1; in the first section of code will show an error message in your IDE telling the user the problem and suggestions of how to fix it, however an IDE isn't perfect and will throw up an alternative such as 'enum' for coding in C++ . This can be easily avoided when checking code and sticking to the coding standards that was agreed upon before the project was started. Most IDE's will show the line of code that the problem has occurred on and will allow the user to step through each bit of code with errors usually displayed as Syntax errors. The main focus is on reading the error message and understanding what the error is telling the user, However, the user should not believe that an error has been identified or solved unless they can recreate it, a simple solution to fix end1; is to replace the 1 (one) with l (letter L) and the error can be easily reproduced, sometimes the errors can be more complicated and expected behaviours are not present, having other programmers is essential in this scenario as another person may be able to spot an error even if it does not present itself in the way of an error message or an error message that the user does not understand, discussing the code with other programmers will help validate that an error is present. 
The next step is to analyse the error, using a bottom up approach, this allows the user to step up through the code to see how big of a problem the error is and whether its code breaking, does the fix of the error result in large sections of code having to be rewritten? After analysis the user will have to prove that the error found within the code is correct and how many other errors are either present or have the potential to be created if the error were to be removed or changed, by confiding in websites such as StackEdit with many users present, it enables a multitude of people to look at the users code and help come up with solutions, this is generally used for small projects. However, for larger programming projects an IDE such as Visual Studio can be used with a debugging tool called Snapshot to take a 'snapshot' of the error, this is essential if the program is live as it does not interrupt the user experience especially if the application is online based. A unique IDE Repl.IT allows the user cloud based programming and debugging, this grants access to the code for the programmer as long as they have internet connection, this is especially useful for remote programming. The final step is implementing the solution and validating the results, with the help of the debugger and any other resources the user has used, they should have all relevant information that is required to fix the error. (Unknown, n.d.)


## **Coding Standards**

Various coding standards are used around the world, many companies use their own standard such as Google with its own GitHub repository dedicated to each of the different codes. A coding standard is a formal way of displaying code in order for the code to be readable and presentable. Its a way of being organized in a fashion where somebody can come back and be able to understand what the original programmer was doing, this consists of;

* Using A, B ,C to represent integers - This makes it easier to understand the code as using any other characters for such a small program would be quite confusing.
* Indentation - This is to ensure that the code has structure and is organised into sections, one can easily define each block of code.
* Consistent use of punctuation - This is so that the program looks even when running.
* Comments on code sections - This is used so that the programmer can look back on their work and be able to understand what each section of code does without having to relearn what was done, this is also helpful for any other programmers who may also work on the code. It stops confusion, such as the case for the example a comment allows the user to easily change between different calculation processes.
* Consistent use of inputs and outputs - for this code cout << endl; was used twice so that each output was separated when running the program, simply for aesthetics.
* Curly brackets - This is used so that the IDE compiler knows what is part of a function and what is not.
* Semicolons -  Are used to end lines so that the compiler knows to look at the next line of code.

Here is an example of the coding standards discussed.

	//Calculation Program made by Luke Farren - 2018
	#include  <iostream>
	using  namespace std;
    int main()
	    {
			    int a, b, c;
			    cout << "Please enter first number to calculate: ";
			    cin >> a; //Input integer.
			    cout << endl; // Uncessary spacing, used for asphetics.
			    cout << "Please enter second number to calculate: ";
			    cin >> b; //Input integer.
			    cout << endl; // Uncessary spacing, used for asphetics.
			    c = a + b; // Change the addition sign to multiplication (*), division (/) or subtraction (-). 
			    cout <<"= " << c << endl; //Output Integer.
		    return  0;
	    } 

[Calculator Link](https://github.com/LukeFarren/Calculator-/blob/master/CalculatorProgramLukeFarren.cpp)


**Bibliography**

Beal, V. (2018). _What is message passing? Webopedia Definition_. [online] Webopedia.com. Available at: https://www.webopedia.com/TERM/M/message_passing.html [Accessed 11 Dec. 2018].

Brownlee, J. (2012). _Clever algorithms_. [United Kingdom]: LuLu.com.

Dutkiewicz, M. (1994). _Algorithm Definition: Prep. by Melanie Dutkiewicz_. MacDonald Dettwiler.

Ferguson, H. R. P.; Bailey, D. H.; and Arno, S. "Analysis of PSLQ, An Integer Relation Finding Algorithm." _Math. Comput._  68, 351-369, 1999.

Rose, M. (n.d.). _What is event-driven application? - Definition from WhatIs.com_. [online] SearchITOperations. Available at: https://searchitoperations.techtarget.com/definition/event-driven-application [Accessed 12 Dec. 2018].

Unknown (n.d.). _Q.What is debugging? Explain the basic steps in debugging? - Solved Assignments_. [online] Sites.google.com. Available at: https://sites.google.com/site/assignmentssolved/mca/semester5/mc0084/6 [Accessed 6 Dec. 2018].

Zandbergen, P. (n.d.). _Object-Oriented Programming vs. Procedural Programming - Video & Lesson Transcript | Study.com_. [online] Study.com. Available at: https://study.com/academy/lesson/object-oriented-programming-vs-procedural-programming.html#transcriptHeader [Accessed 9 Dec. 2018].
