# 💰 React Treasure Hunt Game

### 🤔 Remember
- Pseudocode!!
- Ask clarifying questions

### 📚 User Stories
- As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square.
    - Branch: grid
    - Added an empty div to Square component
      - Styled in css to have a height, width, border
      - imported and called component in App.js
    - Mapped over board array in state to display Square component for each iteration
    - Added styling on a div that surrounds our mapped squares
      - Used flex and wrap, along with setting width.
      - Centered both gameboard and header
    - Passed the value of board to our square component to show question mark
    - Styled question mark to be larger and centered
    (done)

- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array.
    - Branch: alert-index
    - Passed index into square component
    - Made an onClick method that alerts user to what index of the box.
    - Made a method on App.js to pull the information upstream from our child component.  Passed the method down to Square to be invoked when onClick is clicked.
    (done)

- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji.
    - Branch: tree-emoji
    - Destructured board from state so that we could update a single instance to be a tree emoji when clicked
    - Set state once updated
    (done)

- As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
- As a user, I can click on a “Play Again” button that will restart the game.
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).


### 🏔 Stretch Goals
- Consider how to handle a situation where the bomb and the treasure are at the same index.
