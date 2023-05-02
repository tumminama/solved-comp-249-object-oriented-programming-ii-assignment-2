Download Link: https://assignmentchef.com/product/solved-comp-249-object-oriented-programming-ii-assignment-2
<br>
<strong><u>Purpose:</u></strong> The purpose of this assignment is to practice class inheritance, and other Object Oriented Programming concepts such as constructors, access rights, method overriding, etc. The assignment would also allow you to practice the notion of package creation. This assignment contains two parts. You need to complete part I to be able to do part II.

<strong> </strong>

<strong><u>Part I</u> </strong>

<em> </em>

Various publications can be described as follows:




<ul>

 <li>A <strong>PaperPublication</strong> class with the following: <em>price</em> (double type) and <em>number of pages</em> (int type).</li>

</ul>




<ul>

 <li>A <strong>Book </strong>is a <strong>PaperPublication</strong> that in addition has the following: an <em>ISBN</em> (long type), an <em>issue year</em> (int type), a <em>title</em> (String type), and <em>author(s)name</em> (String type).</li>

</ul>




<ul>

 <li>A <strong>ChildrenBook</strong> is a <strong>Book</strong> that in addition has the following: <em>minimum age</em> (int type), which indicates the minimum age that this book is expected for.</li>

</ul>




<ul>

 <li>An <strong>EducationalBook</strong> is a <strong>Book</strong> that in addition it has the following: <em>edition number</em> (int type) and <em>speciality field</em> (String type), such as pharmaceutical, engineering, commerce, etc.</li>

</ul>




<ul>

 <li>A <strong>Journal</strong> is a <strong>PaperPublication</strong> that in addition has the following: <em>issue number</em> (int type) and <em>speciality field</em> (String type), such as pharmaceutical, engineering, commerce, etc.</li>

</ul>




<ul>

 <li>A <strong>Magazine</strong> is a <strong>PaperPublication</strong> that in addition has the following: <em>paper quality</em> (enumeration type that can be: <em>High</em>, <em>Normal</em>, or <em>Low</em>), and <em>issuing frequency</em> (enumeration type that can be: <em>Weekly</em>, <em>Monthly</em>, or <em>Yearly</em>).</li>

</ul>







<u>Part I:</u>




<ol>

 <li>Draw a UML representation for the above mentioned classes hierarchy. Your representation must also be accurate in terms of UML representation of the different entities and the relation between them. You must use a software to draw your UML diagrams (no hand-writing/drawing is allowed).</li>

</ol>




<ol start="2">

 <li>Write the implementation of the above mentioned classes using inheritance and according to the specifications and requirements given below:</li>

</ol>




<ul>

 <li>You must have 4 different Java packages for the classes. The first package will include the <strong>PaperPublication</strong> The second package will include the <strong>Book</strong>, <strong>ChildrenBook</strong> and <strong>EducationalBook</strong> classes. The third package will include the <strong>Journal</strong> class and the last package will include the <strong>Magazine</strong> class.</li>

</ul>




<ul>

 <li>For each of the classes, you must have at least three constructors, a default constructor, a parametrized constructor (which will accept enough parameters to initialize ALL the attributes of the created object from this class) and a copy constructor. For instance the parametrized constructor of the <strong>ChildrenBook</strong> class must accept 7 parameters to initialize the <em>price</em>, the <em>number of pages</em>, the <em>ISBN</em>, the <em>issuing year</em>, the <em>title</em>, the <em>authors name</em>, and the <em>minimum age</em>.</li>

</ul>




<ul>

 <li>An object creation using the default constructor must trigger the default constructor of its ancestor classes, while creation using parametrized constructors must trigger the parametrized constructors of the ancestors.</li>

</ul>




<ul>

 <li>For each of the classes, you must include at least the following methods: accessors, mutators, <strong><em>toString()</em></strong> and <strong><em>equals()</em></strong> methods (notice that you are always overriding the last two methods).</li>

</ul>




<ul>

 <li>The <strong><em>toString()</em></strong> method must display clear description and information of the object (i.e <em>“This Children Book has 57 pages, and costs 28$. It is suitable for age 4 and up …..”</em>).</li>

</ul>




<ul>

 <li>The <strong><em>equals() </em></strong>method must first check if the passed object (to compare to) is null and if it is of a different type than the calling object. The method would clearly return false if any of these conditions is true; otherwise the comparison of the attributes are conducted to see if the two objects are actually equal. You need to add a comment indicating how effective these null verifications inside the method will be in relation to protecting your program from crashing!</li>

</ul>




<ul>

 <li>For all classes, with the exception of the <strong>Book</strong> class, you are required to use the appropriate packages access rights. For the <strong>Book</strong> class for example, you are required to use protected access rights.</li>

</ul>




<ul>

 <li>When accessing attributes from a base class, you must take full advantage of the permitted rights. For instance, if you can directly access an attribute by name from a base class, then you must do so instead of using a public method from that base class to access the attribute.</li>

</ul>




<ol start="3">

 <li>Write a driver program ( that contains the main() method) that would utilize all of your classes. The driver class can be in a separate package or in any of the already existing four packages. In the main() method you must:

  <ul>

   <li>Create various objects from the 6 classes, and display all their information using the <strong><em>toString()</em></strong></li>

   <li>Test the equality of some to the created objects using the <strong><em>equals()</em></strong></li>

   <li>Create an array of 10 <strong>PaperPublication </strong>objects and <u>fill that array with various objects</u> <u>from the 6 classes</u> (each class must have at least one entry in that array).</li>

   <li>Trace(search) that array to find the object that is least expensive (has lowest price) and the one that is most expensive. Display all information of these two objects along with their location (index) in the array.</li>

  </ul></li>

</ol>




<strong><u>Part II</u>  </strong>

<em> </em>

For the requirements of this part,  you need to modify your implementation from Part I as follows:




<ol>

 <li>The classes from part I, must now have the most restrictive (secure/protective) access rights to their attributes. Adjust your implementation from Part I accordingly, and comment on the decision about using restricted access (i.e. what are the tradeoffs).</li>

</ol>




<ol start="2">

 <li>In the driver program of this part, you need to add to the one from part I, another static method (added it above the main()method), called <strong>copyBooks</strong>. The method will take as imput an array of</li>

</ol>

<strong>PaperPublication </strong>(an array of any size) and returns an array of <strong>PaperPublication</strong>. That is to say, the method needs to create an array of the same length as the passed paramter one, copy all books from the passed array to a new array then return it. Your copy of the objects <u>must</u> use the <u>copy</u> <u>constructors</u> of the different listed classes.




<ol start="3">

 <li>In the driver program, create an array of 12 objects (must have at least one from each of the classes), then call the <em>copyBooks()</em> method to create a copy of the that array.</li>

</ol>




<ol start="4">

 <li>Display the contents of both arrays, then add some comments indicating whether or not the coping is correct. If not; you need to explain why it has not been sucessful or as you might expected.</li>

</ol>

<strong> </strong>

<h1>General Guidelines When Writing Programs</h1>

<strong> </strong>

<ul>

 <li>Include the following comments at the top of each class you are writing.</li>

</ul>

// —————————————————–

// Assignment (include number)

// Part: (include Part Number)

// Written by: (include your name(s) and student ID(s))

// —————————————————–




<ul>

 <li>When commenting your code provide on the top a general and clear explanation of what the piece of code is doing; and within that piece of code if there is any method or any loop specify briefly what is doing. Include comments as needed.</li>

 <li>Display clear prompts for the user whenever you are expecting the user to enter data from the keyboard.</li>

 <li>All outputs should be displayed with clear messages and in an easy to read format.</li>

 <li>End your program with a closing message so that the user knows that the program has terminated.</li>

</ul>

<strong> </strong>