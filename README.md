# Soku Solver
Excel based tool for solving Soku Puzzles

## Background
A few years ago I subscribed to the Wall Street Journal and was interested by one of the puzzles I found in the weekend paper. 
Soku is played by placing the numbers 1 through 9 in each of the boxes. Each number can only be used once. The number in each circle is equal to the sum of the surrounding four squares. Each color must total the number shown at the bottom with the same color.

Immediately it became clear to me that there is a better way to solve this problem than simply guessing and checking. It's a classic Linear Programming optimization application. 

I built the following optimization program using the solver in Excel to solve these puzzles. Most computers have Excel and many users are familiar with it (unlike a Python or R script).

## How It Works
A Soku problem is just a series of linear equations. This means that it can be solved algebraically to find the optimal solution. 

A common technique for doing this is using Linear Programming. Specifically here we use the Simplex method. Excel has a built in tool (conveniently called Solver) that can be used to solve this problem. 

I've set up the workbook with formulas that formulate the problem. With the click of a button a macro runs the Solver tool and generates the solution.

Download the Excel file to play around with it.
