Download Link: https://assignmentchef.com/product/solved-cs342-problem-solving-methods
<br>
<h1> Introduction (what is problem solving methods (PSMs)) 10%</h1>

<table width="424">

 <tbody>

  <tr>

   <td width="312">b.     Background (different PSMs techniques)c.     Travel agent as a search problem</td>

   <td width="17"> </td>

   <td width="95">        20%</td>

  </tr>

  <tr>

   <td width="312">i. System component (your system)</td>

   <td width="17"> </td>

   <td width="95">         25%</td>

  </tr>

  <tr>

   <td width="312">ii. Test cases (output of your system)</td>

   <td width="17"> </td>

   <td width="95">         10%</td>

  </tr>

  <tr>

   <td width="312">d. Reference</td>

   <td width="17"> </td>

   <td width="95">          5%</td>

  </tr>

 </tbody>

</table>

<ol>

 <li>Appendix contains the source code of your program 30%</li>

</ol>

<ul>

 <li><strong>Create </strong>one zip file with your document (in pdf format) and code directory</li>

</ul>




<strong><u>System Description:</u></strong>

It is difficult to plan a travel from one city to another city when you are required to use more than one flight, you have to select and arrange the departure and arrival time for every flight in order to minimize the time between each flight and the next so that the total travel time is minimum. The project aims to solve this problem by creating a useful tool to solve the flights search problem, using A* search algorithms.

In other words, you are required to write a program that finds the best flights to reach one city from another city. Given a start city, end city and travel day the system will determine the best way to go from one city to another that minimizes the time. The result will be the <strong>travel plan </strong>that is a complete list of <strong>flights</strong> that a user must use between a series of <strong>cities</strong> to get from a <strong>starting city</strong> to a <strong>destination city</strong>.

<strong><u>System Components:</u></strong>

This program consists of a Planner Engine which  is responsible for:

<ul>

 <li>Taking the query entered by the user.</li>

 <li>Apply the planning algorithm using A* search algorithm to get the best path.</li>

</ul>

<h1> Project Description</h1>




<ul>

 <li>Send the results (travel plan with time needed to reach the destination city) back to the user</li>

</ul>

<strong><u>Project Knowledge</u></strong>

The project contains some knowledge about:

<ul>

 <li>The cities and the different flights between them.</li>

 <li><strong>Cities</strong>: a list of cities included in the system and their positions (in longitude/latitude form), the positions can be used in the heuristic function to calculate the distance between any two cities in order to calculate the expected time to reach one city from another city.</li>

 <li><strong>Flights</strong>: A single flight has a departure time, an arrival time, a flight number, and one or more days that it flies on, you can represent this as:</li>

</ul>

<em>departure / arrival / flight_number / list_of_days </em>

for example:

<em>9:40 / 12:10 / nw600 / [mon, tue, wed, thu, fri] </em>

<ul>

 <li><strong>Flights timetable</strong>: We’ll call all the flights between two cities a timetable. A timetable consists of a departure city, a destination city, and a list of flights, for example:</li>

</ul>

<em>timetable(new_york, san_francisco, [12:10 / 5:00 / nw610 / [mon, tue, wed, thu, fri], 5:30 / 10:15 / united440 / [mon , tue, fri] ]). </em>

<ul>

 <li>The above examples are just for illustration; the knowledge will be represented as predicate <strong><u>Project Input:</u></strong></li>

</ul>

The user will enter the following query to

Print_solution(travel( “Cairo”,”San Fransicsco”,[“Tuesday”,”Wednesday”])) <strong><u>Project Output:</u></strong>

The program will print the result in textual format. For example,

Step 1: use flight 555 from Cairo to London. Departure time 4:30 and arrival time 6:30.

Step 2: use flight 980 from London to New York. Departure time 8:00 and arrival time 15:30. Step 3: use flight united440 from New York to, San Francisco. Departure time 16:30 and arrival time 19:15.

<strong> </strong>

<h2>Topic 2 – Gamification</h2>

<ul>

 <li><strong>Read</strong> <strong>carefully</strong> the given program(s) specifications.</li>

 <li><strong>Write a document that contains the following parts :</strong>

  <ol>

   <li>Introduction (what is Gamification)                                      10%</li>

   <li>Background (How to apply game principles in non-game contexts) 20%</li>

   <li>Development of the described Game</li>

   <li>System component 25% ii. Code listing      30% iii. Test cases (output of your game play)  10%</li>

   <li>Reference                                                                             5%</li>

   <li>Appendix contains the source code of your program 3- <strong>Develop program(s’) </strong>as required in the System Description.</li>

  </ol></li>

</ul>

4- <strong>Create </strong>one zip file with your document (in pdf format) and code directory

<h1>Project Description</h1>

<strong><u>Game Overview</u></strong>

<table width="248">

 <tbody>

  <tr>

   <td width="82">1</td>

   <td width="83">-1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="82">1</td>

   <td width="83">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="82">0</td>

   <td width="83">1</td>

   <td width="83">-1</td>

  </tr>

 </tbody>

</table>

Modified Add the Numbers is a fun logic based game in which you control a box with a numerical value on it. You can move <strong>left</strong>, <strong>right</strong>, <strong>up</strong>, <strong>down</strong> but whatever value is on the box that you replace effects your value. Some will be positive, and some will be negative. A positive will add to your value, but a negative will subtract.

The aim of the game is to get the highest score, given maximum number of movements and minimal score could be achieved. Good Luck and get adding!

<h2><em>Board </em></h2>

<ul>

 <li>Given 3×3 board initially initialize randomly with range [-1, +1].</li>

 <li>Position of player initially down left the board (Green tile in the pic)</li>

</ul>

<h2><em>Rules of Play </em></h2>

<ul>

 <li>The player can only move within the board’s boarder by the move up, down, left or right and he will represented as maximum (Max) player in alpha-beta algorithm.</li>

 <li>The computer will generate a random integer value range between [-1, 1] that will be represented as the minimum (Min) player in alpha-beta algorithm.</li>

 <li>If the player at any corner of board, he can’t move to another corner. Example: If the left most corner he can’t move to the right one if he pressed left button.</li>

 <li>Given the previous figure of the game, if the green tile moves to the right it’s value will be the addition of the old green tile value [0] and the right tile value [1] which will means that the value of the new green tile will be [1] and the value of the old green tile will be replaced by a random value from [-1,1] let’s say computer chose it to be -1 then the next state would look be as represented in the next figure:</li>

</ul>




<table width="248">

 <tbody>

  <tr>

   <td width="83">1</td>

   <td width="83">-1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="83">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="83">-1</td>

   <td width="83">1</td>

   <td width="83">-1</td>

  </tr>

 </tbody>

</table>




<h1>Project Description</h1>

<strong><u>Project Components:</u></strong>

<ol>

 <li><strong><u>Game Engine</u></strong></li>

</ol>

<ul>

 <li>The main process of this engine is initially take the user input and starts to update the game state using the implementation of the alpha-beta algorithm, to select the computer move, and show the board state and so on until the game ends and show the winning state if reached.</li>

</ul>

<ol>

 <li><strong><u>Project Knowledge</u></strong></li>

</ol>

<ul>

 <li>Game state.</li>

 <li>The board state; positions of the tiles as well as the possible moves in the board.</li>

 <li><strong><u>Project Input:</u></strong></li>

 <li>Minimal Level Goal, which choose the computer exceed this value. (for example 10)</li>

 <li>Maximum number of moves, maximum movement to the computer to achieve the goal. (for example 20)</li>

 <li><strong><u>Project Output:</u></strong></li>

</ul>

<ol>

 <li>For each step the current game state should be displayed, using textual representation or in GUI.</li>

 <li>After the game is over, the final results are given including the input values, the current score, and if he wins or fail.</li>

</ol>

<h1>  Project Description</h1>

<strong>Appendix A </strong>

<table width="658">

 <tbody>

  <tr>

   <td width="219">ID</td>

   <td width="219">Name</td>

   <td width="219">Email</td>

  </tr>

  <tr>

   <td width="219"> </td>

   <td width="219"> </td>

   <td width="219"> </td>

  </tr>

  <tr>

   <td width="219"> </td>

   <td width="219"> </td>

   <td width="219"> </td>

  </tr>

  <tr>

   <td width="219"> </td>

   <td width="219"> </td>

   <td width="219"> </td>

  </tr>

 </tbody>

</table>


