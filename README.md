# Connect Four

This was a project at Spiced Academy that I had a lot of fun with. We had to make a 6 x 7 board that would check for horizontal, vertical and diagonal victories. I had to show a Victory popup of some sort and have at least one animation.

I plan on refactoring everything once I have a bit more time.

## Extra Features

From the beginning I wanted to get games saved in local storage. I decided that making a game object would be the best way to achieve this

### The Game Object

The game object in an instance of ConnectFour initiated by calling:
`var game = new ConnectFour(player1Name, player2Name)`
and consists of:

- `gamy.player(1/2)` for both players where the player name, number and score are stored.
- `game.board` for the current board,
- `game.history` where frames from the current game are stored,
- `game.playedGames` where finished games are stored

As well as the methods:

- `game.newBoard()` creating a `new Board()` instance and assignong it to `game.board`
- `game.saveBoard()` pushing the currend frame to `game.history`
- `game.play()` gets the position of the last play (handled in the game login outside of this object) and adds it to the boars array, gets the current player and name and prints it all to the console.

# more coming soon
