# cpsc355-project-part-2-solved
**TO GET THIS SOLUTION VISIT:** [CPSC355 Project Part 2 Solved](https://www.ankitcodinghub.com/product/cpsc355-computing-machinery-i-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116173&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CPSC355 Project Part 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

Objective

You will create a simple single-player game both in C and ARM assembly. This is a two-part project.

Overview

This game is inspired by the retro bomberman game, but it is an oversimplified version. The game consists of a 2D board of hidden rewards and scores. The scores are represented as floating point numbers, positive and negative. The board tiles are randomly populated by these numbers. In addition, the board has an exit tile and reward tiles that double the range of a bomb. When the user uncovers the exit tile, the game is won. The player starts with three lives and a score of zero and a specific number of bombs. S/He chooses a cell to place a bomb. The bomb explodes uncovering the immediate bordering tiles to the bomb. The user’s score is updated as the sum of all the values of the uncovered tiles. If the score becomes negative a life is lost and the number of lives is decremented. If a reward tile is uncovered, the bomb range is doubled: it will be able to uncover the immediately surrounding tiles and their immediately surrounding tiles. If n reward tiles (n $) were found, 2^n layers would be uncovered. Unlike the original game, the bomb never kills the bomberman. The game ends in one of three cases: when the score becomes less than or equal to zero and the lives are zeroed, when the player uncovers the exit tile on the board, or the total number of bombs is exhausted before uncovering the exit tile. When the user starts a new life, the total number of bombs is maintained from the previous life and the score is zeroed. There is no need for a graphical interface.

Details

The user starts the game by specifying a player name and the dimensions of the game board. These will be NM grids. The minimum value of N and M is 10 and there is no maximum, as long as the game board can be fit on the screen. For example, the following command line invocation starts the game with a 100×200 grid:

./mygame.o bomberman 100 200

The grid is then initialized with random floating numbers with two precision points, ensuring that around 40% of the cells are negative, around 40% of cells are positive and the remaining cells, around 20% are bonus pack tiles including the exit tile ‘*’ . These numbers should be non-zero with a maximum absolute value of 15. You must use bitwise arithmetic to calculate the modulus of the random numbers.

To help with grading, display the uncovered game board, showing all the contents of the tiles and stating the ratio of negative tiles, positive tiles and special tiles. Therefore, if the board is 3×4 (Remember: the minimum value of N and M is 10 and there is no maximum) your program should display something like the following before the actual game starts:

1.00 -2.10 $ 0.50

14.00 -7.20 -1.10 12.00

-0.70 * 5.00 -4.01

Negative numbers 5/12 = 41.67%

Positive numbers 5/12 = 41.67%

Special tiles 2/12 = 16.67%

The normal (covered) game board is then displayed. We will give an example using 55 grid (such a board size is too small to result in a meaningful game). The initial screen will look like the following (note that the number of bombs needs to be appropriate for the game board size):

XXXXX

XXXXX

XXXXX

XXXXX

XXXXX

Lives: 3

Score: 0

Bombs: 3

Prompt the user to choose a tile to place the bomb by entering its coordinates, such as:

Enter bomb position (x, y): 0 1

The move is applied, and the resulting game state is shown again (+ indicates a positive score and – a negative score). For example:

Total uncovered score of 5.23 points

++-XX

-++XX

XXXXX

XXXXX

XXXXX

Lives: 3

Score: 5.34

Bombs: 2

Bang!! Your bomb range is doubled

Total uncovered score of 5.23 points

++-XX

-$+XX

XXXXX

XXXXX

XXXXX

Lives: 3 Score: 5.34

Bombs: 2

Since a $ is uncovered, the next bomb will have a double-range effect. This effect lasts for one bomb only. The exit tile is represented using the * symbol.

The user can choose at any time to exit the game. When the game ends with a win or a loss, the player’s name, score, and duration of the play are recorded in a log file. A user can also ask to display the top n scores before or after any game, including player names and duration.

Modularity

Your code must be divided into functions as appropriate. At a minimum, you must define the following functions (we are not showing all necessary arguments):

– initializeGame(*board)

– randomNum(n,m,neg); n and m are the lower and upper bounds for the random number; the generated number is negative if neg is true.

– displayGame(*board)

– calculateScore(), returns overall score

– logScore()

– exitGame()

– displayTopScores(n)

Re-create the same game entirely in ARMv8 assembly. For this part, we suggest that you implement the game first without floating-point numbers. Then, you can add this feature at the end of the semester. If your code is modular enough. It should only require you to replace a few subroutines. Make sure to use service calls for file I/O at least once in your program Split your source code into two files at least.

Submission

-12.5% for each late day or portion of a day for the first two days

-25% for each additional day or portion of a day after the first two days

Academic Misconduct

This project is to be done by individual students: your final submission must be your own original work. Teamwork is not allowed. Any similarities between submissions will be further investigated for academic misconduct. While you are encouraged to discuss the project with your colleagues, this must be limited to conceptual and design decisions. Code sharing by any means is prohibited, including looking at someone else’s paper or screen. The submission of compiler generated assembly code is absolutely prohibited. Any re-used code of excess of 5 lines in C and 10 lines in assembly (10 assembly language instructions) must be cited and have its source acknowledged. Failure to credit the source will also result in a misconduct investigation.

C- Requirement

As per the course syllabus, a cumulative C- must be achieved in the project in order to achieve a C- in the course.

Computing Machinery I

Project Rubric

Student:__________________________________________

Item Max Points Points

Code compiles including separate compilation

5

Program displays uncovered board and percentage of negative numbers

5

Game logic

30

Use of floating-point numbers

10

User interface (input validation, implementing all features)

10

Random numbers

10

Use of binary arithmetic (mod with random numbers)

5

Modularity and macros (macros: part 2)

10

Command-line arguments

5

Passing array parameters by reference

5

Code readability (documentation)

5

Bonus (surprise packs)

10 (bonus)
