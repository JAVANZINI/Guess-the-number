# Guess-the-number

RESTful API developed using Java as an end point for users playing the game 

Developed Server Logic and Unit Tests to assure continued functionality 

Used JDBC Template to interact with the MySQL Database 


Game  "Bulls and Cows". In each game, a 4-digit number is generated where every digit is different. For each round, the user guesses a number and is told the exact and partial digit matches.

 REST endpoints: 
"begin" - POST – Starts a game, generates an answer, and sets the correct status.Return a 201 CREATED message as well as the created gameId.
"guess" – POST – Makes a guess by passing the guess and gameId in as JSON. The program  calculate the results of the guess and mark the game finished if the guess is correct. It returns the Round object with the results filled in.
"game" – GET – Returns a list of all games. Games in-progres do not display their answer.
"game/{gameId}" - GET – Returns a specific game based on ID. In-progress games do not display their answer.
"rounds/{gameId} – GET – Returns a list of rounds for the specified game sorted by time.
