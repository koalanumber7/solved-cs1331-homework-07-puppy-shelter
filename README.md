Download Link: https://assignmentchef.com/product/solved-cs1331-homework-07-puppy-shelter
<br>
<strong>r</strong>

<h1>Problem Description</h1>

You are walking down the street one day when you stumble across a puppy. Like, literally stumble. And so like the guilty good person you are, you take the now-injured puppy and take him to the nearby veterinarian, who directs you to a local puppy shelter. At the puppy shelter, you start chatting with the owner, and before you know it you’ve volunteered to write code for the puppy shelter! You will help the owner modernize his store by writing a Java program that allows him to track each puppy in his care.

<h1>Solution Description</h1>

For this assignment, create a file with the following name:

<ul>

 <li>java</li>

</ul>

<strong>Puppy Class:</strong>

<em>Instance Variables</em>

<ul>

 <li>String name holds the name of the puppy. It should have private access.</li>

 <li>int age holds the age of the puppy. It should have private access.</li>

 <li>int health holds the health of the puppy. It should have private access.</li>

</ul>

<em>Constructors</em>: Be sure to use constructor chaining.

<ul>

 <li>Puppy(String name, int age, int health)</li>

 <li>Puppy(String name)

  <ul>

   <li>Assign the puppy a random age between 0 and 15, inclusive.</li>

   <li>Assign the puppy a random health between 5 and 35, inclusive.</li>

   <li>Again, make sure to use constructor chaining! HINT: Try creating a static Random field that you can use.</li>

  </ul></li>

</ul>

<em>Methods</em>:

<ul>

 <li>Correct public getters &amp; setters for name, age, and health</li>

 <li>String toString() Returns “[name]: a puppy [age] years old with [health] health”</li>

 <li>boolean canAdopt() Returns true when the puppy can be adopted and false otherwise. A puppy can be adopted if its health is 50 or above.</li>

 <li>void fetch() Increases the puppy’s health by 1 (because it got exercise)</li>

 <li>void fetch(boolean inside) The parameter inside signals whether or not you’re playing fetch inside or outside. If inside, increase health by 5. If not inside, increase health by 10.</li>

 <li>void fetch(int distance) Distance represents how far the toy is thrown. Increase the puppy’s healthy by distance divided by 10. Truncate decimals if necessary.</li>

</ul>

<strong>Testing your code:</strong>

If you want to test out your own code before submitting we recommend creating a separate java file and implementing a main method there. You can then create new animals and test your methods. Below is some sample testing code. <strong>These tests are not comprehensive!</strong>

Puppy pup = <strong>new </strong>Puppy(“pup”);

System.out.println(“age: ” + pup.getAge());

System.out.println(“health: ” + pup.getHealth());

pup.fetch(<strong>true</strong>);

System.out.println(“Play fetch outside”);

System.out.println(“health: ” + pup.getHealth());

This could print out age: 15 health: 7

Play fetch outside health: 12

Feel free to create your own tests in the main method! Try to write tests for the remaining methods in the file!

<h1>Rubric</h1>

<ul>

 <li>[100]</li>

 <li>[5] Instance variables</li>

 <li>[10] Constructor with three parameters assigns properly</li>

 <li>[10] Constructor with one parameter assigns properly</li>

 <li>[10] Creates random values correctly</li>

 <li>[10] Constructor Chaining</li>

 <li>[10] Setters &amp; Getters correct for name, age, and health</li>

 <li>[10] toString()</li>

 <li>[5] canAdopt()</li>

 <li>[10] fetch()</li>

 <li>[10] fetch(boolean) <strong>– </strong>[10] fetch(int)</li>

</ul>

<h1>Allowed Imports</h1>

<ul>

 <li>To prevent trivialization of the assignment, you are only allowed to import the following class:</li>

</ul>

<strong>– </strong>java.util.Random

<h1>Javadocs</h1>

For this assignment, you will be commenting your code with Javadocs. Javadocs are a clean and useful way to document your code’s functionality. For more information on what Javadocs are and why they are awesome, the <a href="http://www.oracle.com/technetwork/java/javase/documentation/index-137868.html">online overview</a> for them is extremely detailed and helpful.

You can generate the javadocs for your code using the command below, which will put all the files into a folder called javadoc:

$ javadoc *.java -d javadoc

The relevant tags that you need to include are @author, @version, @param, and @return. Here is an example of a properly Javadoc’d class:

<table width="632">

 <tbody>

  <tr>

   <td width="632"><strong>import </strong>java.util.Scanner;<em>/**</em>* This class represents a Dog object<em>.</em>* <strong>@author </strong>George P<em>. </em>Burdell* <strong>@version </strong><em>1.0</em><em>*/ </em><strong>public class </strong>Dog {<em>/**</em>* Creates an awesome dog <em>(</em>NOT a dawg<em>!) */</em><strong>public </strong>Dog() { …}<em>/**</em>* This method takes in two ints and returns their sum* <strong>@param a </strong>first number* <strong>@param b </strong>second number <em>* </em><strong>@return </strong>sum of a and b<em>*/</em><strong>public </strong>int add(int a, int b) {…}}</td>

  </tr>

 </tbody>

</table>

A more thorough tutorial for Javadocs can be found <a href="https://cs1331.gitlab.io/cs1331-style-guide.html">here</a>. Take note of a few things:

<ol>

 <li>Javadocs are begun with /** and ended with */.</li>

 <li>Every class you write must be Javadoc’d and the @author and @verion tag included. The comments for a class should start with a brief description of the role of the class in your program.</li>

 <li>Every non-private method you write must be Javadoc’d and the @param tag included for every method parameter. The format for an @param tag is @param &lt;name of parameter as written in method header&gt; &lt;description of parameter&gt;. If the method has a non-void return type, include the @return tag which should have a simple description of what the method returns, semantically.</li>

</ol>


