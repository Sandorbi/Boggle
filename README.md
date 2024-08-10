# Boggle
Boggle is a board game with a 4x4 square grid of letter cubes where players try to make words by connecting letters on adjacent cubes.
Letter cubes are 6-sided dice with a letter on each side rather than a number.
The goal is to find words on the board by tracing a path through neighboring letters. Two letter cubes are neighbors if they are next to each other horizontally, vertically, or diagonally. Therefore there are up to eight neighbors near a cube. Each cube can be used at most once in a given word.

In the real-life version of this game, all players work at the same time, listing the words they find on a piece of paper. But in the version we will write, a single human player will play a single turn against an omniscient computer opponent.

The human player plays first, entering words one by one. Your code verifies that the word is is at least 4 letters long, then uses backtracking to see if the word can be made using letters on the board, using any cube at most once.

Once the player has found as many words as they can, the computer player takes a turn. The computer searches through the board using recursive backtracking to find all the possible words that can be formed. The computer's algorithm is similar to the human's, but rather than verifying the existence of a single word in the board, you are exhaustively finding the set of all possible words.
