# Game_Snake
This is a recreation and modification of the game Snake using JavaSwing 

## Notable Concepts Used

  ### 2D Array 
     2D Array used to randomly generate where fruits should be placed on the screen.This 2D array is helpful when reading and
     writing to file. Another is used to store fruits to be printed to the screen. Fruit 2D array stores fruits and its
     properties, the fruits position in the 2D array is used to see if it intersects with the head of the snake.

  ### Inheritance and Subtyping
    Fruit interface is used and contains the functions eat and draw. It has two subtypes apples and bananas.
    The eat function in Apple lengthens ths snake by one square. That of Banana, lengthens the snake by 2
    squares. Dynamic dispatch is used when the fruit array is looped through in the move function and eaten if
    it collides with the head. The 2D array is of fruits and it is not specified which one when calling the eat
    function.

  ### File IO 
    File I/O is used to store a users progress in the game. They are then allowed to close the game and resume it
    when they reopen the game. The file stores the game state including the score, the snake and its properties as well
    as the position where a fruit is stored in the 2D array and what fruit is stored there.

  ### Collection
    A linked list is being used to store the moving parts of the snake. This was an appropriate structure to use to keep
    moving the snake. The tail could be continuously moved and added to the head to simulate a snake like motion.
  
## File Descriptions
    Fruit.java - Interface that defines the methods eat and draw which are can be called on a fruit.
    Apple.java - subtype of the fruit interface that eats a snake by making it a block longer. Draw an apple.
    Banana.java - subtype of the fruit interface that eats the snake by making it 2 times longer. Draw a Banana.
    Direction.java - An enumeration storing the direction UP,DOWN,LEFT,RIGHT
    Square.java - stores the basic unit of the snake. A square that has an x, y and color.
    data.txt - file that is being written to and read from
    PopUpInstructions.java - class creating and storing the instructions of the game
    GameCourt.java - where the game is played, resume, pause, same and continue is handled
    RunSnake.java - where the snake is built, it's movement is controlled, its drawn and the direction is set and collisions
    are handled
    Point.java - stores an x and y value in the form of a point
    RunSnake.java - where the game frame and panels are created and the game is displayed  to the frame

## Game Demo 
Here is a link to a video demo of the Game: 
https://drive.google.com/file/d/1oMnSaXc2HNUx0fyTpORPjFXK82IsH7cy/view?usp=sharing 

<img width="555" alt="Screenshot 2023-05-26 at 4 07 35 PM" src="https://github.com/Sukya1/Game_Snake/assets/90349473/1015be38-6e06-483e-be41-9c21a8f78e08">
