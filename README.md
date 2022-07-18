# Goal

The goal of this task is to implement the `Find Challenge`. It's a modification of the [word search game](https://lovattspuzzles.com/online-puzzles-competitions/play-daily-word-search-puzzle-online/). Instead of finding a list of words in the grid, the user needs to find all possible translations of one given word.

# Specification

You are given a word `source` and a list of translations `targets`. Your task is to display the word `source` and a grid of letters that contains all the `targets`. The user's task is to find all the translations in the grid. The user selects a word by clicking on the first letter, dragging the mouse to the last letter, and releasing the mouse; if the user drags the mouse to a letter and then away from it, it should deselect only that specific letter. If 

When the selected word is a valid translation of the source word, it should stay highlighted. Otherwise, the selection should disappear; and if the user drags the selection away from the game (i.e. away from the browser area), it should also be considered a deselection. 

After all targets have been found, the app should display a new grid and a new source word. Your app's source data should be the contents of [this file](https://github.com/finmid/code-challenge-fe/blob/main/find-challenge). Each line contains a JSON object.

### Here is a spec for the file format:

- `word:` the source word.
- `character_gri:` the character grid to be shown.
- `word_locations:` a dictionary where each key is a list of coordinates in the format: x1, y1, x2, y2, ..., xn, yn and the value is the target word in that location.

### Requirements:

- Target words may appear horizontally, vertically, or diagonally. User selection movement must be limited to those directions.
- Some `source` words may have more than one `target`. The user needs to select both to mark that one as completed.
- All code must be written in TypeScript.
- React must be used as well.

# Evaluation

Your code will be evaluated by the following criteria: 

1. Correctness: Are all the requirements fulfilled? Is the user able to select/deselect the words, and complete the game?
2. Usability: Is it easy to select words with the mouse? Is the UI responsive? Is the UX good?
3. Code quality: Is the code well organized and easily readable? Is the game logic isolated from the view logic?

## Bonus

You are not required to tackle these, but if you do we'll take that into consideration:
- Unit, render, and e2e tests
- Deployment configuration (CI/CD, docker, etc)
- Pretty UI
