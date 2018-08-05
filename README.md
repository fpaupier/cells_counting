# Counting red blood cell in blood smear

## Goal of the project

The goal of this project is to count the number of blood cells in a 2D image
of a blood smear.

## Steps
I use several steps of image pre-processing to obtain a binary image from which it is
easy to count the cells by counting the white zones in the image.

Many methods are available to solve this problems. I  present some of them and
compare the results before concluding.

## Most effective method
The most accurate method I found is a pattern matching approach.
I take a reference cell, and convolute it to the image. Higher intensity zones corresponds to cells center.
Then I apply a threshold at a given percentage of the histogram to get a binary image where the cells
are white circles and the rest is black.
Then, I use one of MatLab function to count the white zones in the binary image.


## Notes
This project was part of my Master Of Science _Major in statistics_ at Centrale Nantes engineering school.
