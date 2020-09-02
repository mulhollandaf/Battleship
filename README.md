# Battleship

The goal is to win in the fewest average shots

Battleship is played on a 10 X 10 grid
The ships sizes are 5 4 3 3 2

Players are expected to create their own shooter that implements this interface

interface BattlesihpShooter {
    fun shoot(lastResult: Int) : Pair<Int, Int>
}

The game will call the call the shooter until all the boats are sunk. When the function is called it will send one paramter, the last result. The is the status of the last shot.

0 - Miss
1 - Hit
2 - Sink

The first shot will send a 0.

The game will be played 1000 times and the average number of shots will be your score. The lower the better.

Suggested steps
1. Shoot every square
2. Shoot every other diagonal
3. Shoot in a more complex pattern
