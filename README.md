# NGram Hangman

This is an implementation of a N-Gram model that plays (makes informed guesses in) the Hangman game by itself.

## The Problem

The Hangman game is a classic word puzzle where the goal is to guess a hidden word by suggesting letters within a limited number of tries (6 in this case). This project enhances the traditional approach by using statistical models to predict the next letter, thereby increasing the chances of correctly guessing the word.

## Approach

### N-Gram Model

The core algorithm uses N-gram models, which predict the next Hangman game letter by analysing statistical patterns in letter sequences within words. This method aids informed guessing based on revealed letters and common word patterns in the English language.

#### Why N-Gram Model?

1.  **Contextual Prediction**: The N-gram model predicts letters based on surrounding context, capturing common letter patterns in the English language.
2.  **Efficiency**: Training the N-gram model is efficient, relying on statistical inferences which are faster to compute.
3.  **Improved Accuracy**: Compared to simple frequency analysis, N-gram models provide more accurate predictions by considering the dependency between letters.
4.  **Avoids Overfitting**: Unlike decision trees, which risk overfitting and are computationally intensive, N-gram models are straightforward and robust.

### Implementation

The implementation preprocesses a given set of words to build up to a 7-gram model. This involves storing the frequency of all sequences of letters, of lengths 1 to 7, appearing in the dictionary of words. The model then uses these frequencies to predict the most probable next letter during the game.

### Accuracy

-   **Practice Games**: Achieved an accuracy of approximately 64% to 66% over 500 practice games.
-   **Recorded Games**: Maintained an accuracy of 62.5% over 1000 recorded games.

## Thanks :)
