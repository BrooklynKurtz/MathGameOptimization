# MathGameOptimization
Optimizing a math-based game of my own design

--"Summarize the project and what problem it was solving."

This program computes the optimal solution for a math-game to be played with students learning arithmetic (but it's also kinda fun, so go ham).
I came up with this back when I was a teacher, and students quite liked it.

The game boils down to this:

Each player starts off with four operation cards: addition, subtraction, multiplication, and division

Then each player is dealt four integer cards, each representing an integer from 1 - 10

Then, a d20 is rolled to determine the target value

Each player has two opportunities to swap out up to two of their integer cards at a time for new cards

Once each player has passed twice, the players lay down their cards to form an arithmetic expression.

They do this by selecting three of their four operations and alternating between integer and operation, like so:

    Integer - Operation - Integer - Operation - Integer = Operation - Integer

Players then evaluate the expressions using appropriate order of operations. The winner is the player with the expression which evaluates closest to the target value.


This program finds the optimal arithmetic expression for a given set of integers and target value.

--"What did you do particularly well?"

Overall, I think the code looks nice and it definitely functions as intended. My favorite bit is the GetPermutations function, which was a pain to work out.
My original idea for this function relied on some group theory to find a minimal set of permutations, but this ended up being a bit much to code. Eventually,
I came up with this solution, which essentially matches my original idea but being much more straightforward to implement.

--"Where could you enhance your code? How would these improvements make your code more efficient, secure, and so on?"

The first major enhancements that I would make to this code involve moving a lot of the functions into classes. This is actually how the code originally worked,
but I had a hard time working out how to break this up into discrete objects. So, I focused on getting the code to work first. The main benefit of building this into a class
is that it will enhance the potential utility of the code. There are tons of applications for finding permutations of a set of objects. Eventually, I would also like to 
wrap this all up in a snazzy GUI.

--"Which pieces of the code did you find most challenging to write, and how did you overcome this? What tools or resources are you adding to your support network?"

My god, working out how to build the permutations and evaluating the equations was super tough. I spend more time than I should have working on those bits. Eventually, I worked through the
difficulties, though. Lots of Google searches. I found a few resources for some of the C++ modules I had to pull in, which cleared up a few things. GitHub, cplusplus.com, and cppreference.com were
SUPER helpful here.

--"What skills from this project will be particularly transferable to other projects or course work?"

I have a better handle now of how to read the reference materials on cplusplus.com, which will be helpful when I inevitably need to pull from that resource again. Honestly, the biggest skill
I gained from this project is honing my ability to work through a complex coding challenge. Lots of patience required.

--"How did you make this program maintainable, readable, and adaptable?"

Comments, whitespace, and keeping things modular make the program readble and maintainable. Adaptability wasn't an immediate concern when I built this, but that can be added
and enhanced with future updates. Consolidating functionality into classes, for example.
