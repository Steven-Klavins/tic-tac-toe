This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

Tic-tac-toe, also known as noughts and crosses, or Xs and Os is a game for two players, X and O, who take turns marking the spaces in a 3×3 grid. The player who succeeds in placing three of their marks in a horizontal, vertical, or diagonal row is the winner.

[Play the game](http://tic-tac-toe-sk.surge.sh/)

This project is an adaption of the official React [Tutorial](https://reactjs.org/docs/create-a-new-react-app.html)

## Tic Tac Toe

<p align="center">
<img src="Screenshot_TTT.png" alt="screenshot" width="600"/>
</p>

### How it works

As previously mentioned this is an adaptation of the official React tutorial. The game is made of 3 key components, a square component, a grid component, and the game component itself. The square component is essentially a button with styling, the grid component passes the button an onclick event as a prop which instructs when and what to update.

The grid component handles the majority of the logic of the game and renders the square component in 3 rows of 3 (9 squares in total). When a player clicks a square an 'X' or an 'O' is added to an array and rendered to the grid. Players turns are tracked by a boolean which is flipped each round, if the boolean is true an X will be rendered, if its false it renders an O. 

Each round the game checks to determine if there's a winner, in the event there is the onclick method will be disabled and the player will need to hit the reset button and clear the array to start over. This is one of the features I added as it was not covered in the tutorial (at least not as far as I read), the second biggest difference would be the CSS styling which I felt gave the game some charm.

### Future improvements

In the future, I feel it would be a nice touch to perhaps animate the game with transitions, I don't think it would be too troublesome to achieve with something like Framer Motion. However, what was important to me was the game logic itself worked first. I am also tempted to convert this project to a react native application as I feel it would be fairly easy to adapt this for mobile devices.
