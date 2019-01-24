# Elevens 8

Follow the instructions provided for Activity 8 in the student lab guide. This is more of an exploratory lab, so you will not need to copy any of your previous code into the repo. Answer the questions from the Student Guide in this document and ensure that you save and push the repo. You have one week to complete this lab.

1. Discuss the similarities and differences between *Elevens*, *Thirteens*, and *Tens*.

    * Answer: All three games involve boards, cards, decks, point values, and suits. Elevens used a nine-card board, thirteens uses a ten-card board, and tens uses a thirteen-card board. To win a game of Elevens, cards must add up to a point value of eleven, and thirteen and ten for Thirteens and Tens respectively.

2. As discussed previously, all of the instance variables are declared in the `Board` class. But it is the `ElevensBoard` class that “knows” the board size, and the ranks, suits, and point values of the cards in the deck. How do the `Board` instance variables get initialized with the `ElevensBoard` values? What is the exact mechanism?

    * Answer: Inheritance - ElevensBoard extends the Board class, meaning it is a subclass of Board and can access the same instance variables through the constructor.

3. Now examine the files `Board.java` and `ElevensBoard.java`, found in this repository. Identify the `abstract` methods in `Board.java`. See how these methods are implemented in `ElevensBoard`. Do they cover all the differences between *Elevens*, *Thirteens*, and *Tens* as discussed in question 1? Why or why not?

    * Answer: The abstract methods are isLegal and anotherPlayIsPossible. The same abstract methods are accessed in each subclass but are overridden in their respective subclasses to work differently depending on the rules of the game. isLegal and anotherPlayIsPossible differentiate the difference between the three games by covering the differences in point value indirectly accounting for the size of the board.
