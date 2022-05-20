# Goal

The goal of this task is to implement the `Find Challenge`. It's a modification of the [word search game](https://lovattspuzzles.com/online-puzzles-competitions/play-daily-word-search-puzzle-online/). Instead of finding a list of words in the grid, the user needs to find all possible translations of one given word.

# Specification

You are given a word `source` and a list of translations `targets`. Your task is to display the word `source` and a grid of letters that contains all the `targets`. The user's task is to find all the translations in the grid. The user selects a word by clicking on the first letter, dragging the mouse to the last letter, and releasing the mouse. When the selected word is a valid translation of the source word, it should stay highlighted. Otherwise, the selection should disappear. After all targets have been found, the app should display a new grid and a new source word. Your app's source data should be the contents of [this file](https://github.com/finmid/code-challenge-fe/blob/main/find-challenge). Each line contains a JSON object.

### Here is a spec for the file format:

- `word:` the source word
- `character_gri:` the character grid to be shown
- `word_locations:` a dictionary where each key is a list of coordinates in the format: x1, y1, x2, y2, ..., xn, yn and the value is the target word in that location.

### Additional requirements:

- Target words may appear horizontally, vertically, or diagonally
- All code must be written in TypeScript
- Please use React as well

# Evaluation

Your code will be evaluated by the following criteria: 

1. Usability: Is it easy to select words with the mouse? Is the UI responsive?
2. Correctness: Are all the requirements fulfilled?
3. Cleanliness: Is the code well organized and easily readable?

