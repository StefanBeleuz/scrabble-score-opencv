# Scrabble score calculator

## Objective

The goal of this project is to develop an automatic system for scoring words placed on the Scrabble board.

## Data description

The `train_data` directory contains data (images and annotations files) for 5 games, where each game has 20 turns.

The first two games consist of images with regular views, the images are taken with the phone placed parallel above the board, with minor scale changes and rotations. The third game consists of images with rotated views, the images are taken with the phone placed parallel above the board, but at some non negligible rotation wrt the board. The fourth game consists of images with perspective views, the images are taken with the phone tilted wrt the board. The fifth game consists of images with mixed views.

The ground-truth annotations files contain for each turn the following information:

- the positions of tiles added to the board, taken in the order from left to right and from top to down. For specifying a position on the board use numbers 1-15 for rows and letters A-O for columns;
- the tile letter placed at the corresponding position on the board;
- the total score obtained in the current turn.

## Requirements

The task is to write a program that automatically solves the task of extracting information of the current turn depicted in a test image. For each test image you have to output the corresponding information similar to the annotation files, thus specifying the positions of newly added tile letters to the board, which letters are placed at the corresponding position on the board and the total score obtained in the current turn.

## Implementation

View `scrabble_score.md` for details about implementation. 