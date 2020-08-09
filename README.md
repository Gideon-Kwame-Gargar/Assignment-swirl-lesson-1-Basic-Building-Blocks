# Assignment-swirl-lesson-1-Basic-Building-Blocks
Select 1, 2, or 3 and press Enter 

1: Continue.
2: Proceed.
3: Let's get going!

Selection: 3

| You can exit swirl and return to the R prompt (>) at any time by pressing the Esc
| key. If you are already at the prompt, type bye() to exit and save your progress.
| When you exit properly, you'll see a short message letting you know you've done
| so.

| When you are at the R prompt (>):
| -- Typing skip() allows you to skip the current question.
| -- Typing play() lets you experiment with R on your own; swirl will ignore what
| you do...
| -- UNTIL you type nxt() which will regain swirl's attention.
| -- Typing bye() causes swirl to exit. Your progress will be saved.
| -- Typing main() returns you to swirl's main menu.
| -- Typing info() displays these options again.

| Let's get started!

...install_from_swirl("R Programming")

| Please choose a course, or type 0 to exit swirl.

1: R Programming
2: Take me to the swirl course repository!

Selection: 1

| Please choose a lesson, or type 0 to return to course menu.

1: Base Graphics
2: Basic Building Blocks
3: Dates and Times

Selection: 2

  |                                                                           |   0%

| In this lesson, we will explore some basic building blocks of the R programming
| language.

...

  |==                                                                         |   3%
| If at any point you'd like more information on a particular topic related to R,
| you can type help.start() at the prompt, which will open a menu of resources
| (either within RStudio or your default web browser, depending on your setup).
| Alternatively, a simple web search often yields the answer you're looking for.

...

  |====                                                                       |   5%
| In its simplest form, R can be used as an interactive calculator. Type 5 + 7 and
| press Enter.

> 5+7
[1] 12

| Perseverance, that's the answer.

  |======                                                                     |   8%
| R simply prints the result of 12 by default. However, R is a programming language
| and often the reason we use a programming language as opposed to a calculator is
| to automate some process or avoid unnecessary repetition.

...

  |========                                                                   |  11%
| In this case, we may want to use our result from above in a second calculation.
| Instead of retyping 5 + 7 every time we need it, we can just create a new variable
| that stores the result.

...

  |==========                                                                 |  13%
| The way you assign a value to a variable in R is by using the assignment operator,
| which is just a 'less than' symbol followed by a 'minus' sign. It looks like this:
| <-

...

  |============                                                               |  16%
| Think of the assignment operator as an arrow. You are assigning the value on the
| right side of the arrow to the variable name on the left side of the arrow.

...

  |==============                                                             |  18%
| To assign the result of 5 + 7 to a new variable called x, you type x <- 5 + 7.
| This can be read as 'x gets 5 plus 7'. Give it a try now.

> x <- 5+7

| Nice work!

  |================                                                           |  21%
| You'll notice that R did not print the result of 12 this time. When you use the
| assignment operator, R assumes that you don't want to see the result immediately,
| but rather that you intend to use the result for something else later on.

...

  |==================                                                         |  24%
| To view the contents of the variable x, just type x and press Enter. Try it now.

> x
[1] 12

| You are amazing!

  |====================                                                       |  26%
| Now, store the result of x - 3 in a new variable called y.

> y <- x-3

| Excellent job!

  |======================                                                     |  29%
| What is the value of y? Type y to find out.

> y
[1] 9

| You are quite good my friend!

  |========================                                                   |  32%
| Now, let's create a small collection of numbers called a vector. Any object that
| contains data is called a data structure and numeric vectors are the simplest type
| of data structure in R. In fact, even a single number is considered a vector of
| length one.

...

  |==========================                                                 |  34%
| The easiest way to create a vector is with the c() function, which stands for
| 'concatenate' or 'combine'. To create a vector containing the numbers 1.1, 9, and
| 3.14, type c(1.1, 9, 3.14). Try it now and store the result in a variable called
| z.

> z <- c(1.1, 9, 3.14)

| That's the answer I was looking for.

  |============================                                               |  37%
| Anytime you have questions about a particular function, you can access R's
| built-in help files via the `?` command. For example, if you want more information
| on the c() function, type ?c without the parentheses that normally follow a
| function name. Give it a try.

> ?c

| You nailed it! Good job!

  |==============================                                             |  39%
| Type z to view its contents. Notice that there are no commas separating the values
| in the output.

> z
[1] 1.10 9.00 3.14

| All that practice is paying off!

  |================================                                           |  42%
| You can combine vectors to make a new vector. Create a new vector that contains z,
| 555, then z again in that order. Don't assign this vector to a new variable, so
| that we can just see the result immediately.

> c(z,555,z)
[1]   1.10   9.00   3.14 555.00   1.10   9.00   3.14

| Keep up the great work!

  |==================================                                         |  45%
| Numeric vectors can be used in arithmetic expressions. Type the following to see
| what happens: z * 2 + 100.

> z*2+100
[1] 102.20 118.00 106.28

| You are quite good my friend!

  |====================================                                       |  47%
| First, R multiplied each of the three elements in z by 2. Then it added 100 to
| each element to get the result you see above.

...

  |======================================                                     |  50%
| Other common arithmetic operators are `+`, `-`, `/`, and `^` (where x^2 means 'x
| squared'). To take the square root, use the sqrt() function and to take the
| absolute value, use the abs() function.

...

  |=======================================                                    |  53%
| Take the square root of z - 1 and assign it to a new variable called my_sqrt.

> my_sqrt<-sqrt(z-1)

| You're the best!

  |=========================================                                  |  55%
| Before we view the contents of the my_sqrt variable, what do you think it
| contains?

1: a vector of length 3
2: a vector of length 0 (i.e. an empty vector)
3: a single number (i.e a vector of length 1)

Selection: 1

| You are doing so well!

  |===========================================                                |  58%
| Print the contents of my_sqrt.

> print(my_sqrt)
[1] 0.3162278 2.8284271 1.4628739

| One more time. You can do it! Or, type info() for more options.

| Just type my_sqrt and press Enter to view its value.

> my_sqrt
[1] 0.3162278 2.8284271 1.4628739

| That's a job well done!

  |=============================================                              |  61%
| As you may have guessed, R first subtracted 1 from each element of z, then took
| the square root of each element. This leaves you with a vector of the same length
| as the original vector z.

...

  |===============================================                            |  63%
| Now, create a new variable called my_div that gets the value of z divided by
| my_sqrt.

> my_div<-z/my_sqrt

| All that hard work is paying off!

  |=================================================                          |  66%
| Which statement do you think is true?

1: The first element of my_div is equal to the first element of z divided by the first element of my_sqrt, and so on...
2: my_div is a single number (i.e a vector of length 1)
3: my_div is undefined

Selection: 1

| You're the best!

  |===================================================                        |  68%
| Go ahead and print the contents of my_div.

> print(my_div)
[1] 3.478505 3.181981 2.146460

| That's not exactly what I'm looking for. Try again. Or, type info() for more
| options.

| Type my_div and press Enter to see its contents.

> my_div
[1] 3.478505 3.181981 2.146460

| Nice work!

  |=====================================================                      |  71%
| When given two vectors of the same length, R simply performs the specified
| arithmetic operation (`+`, `-`, `*`, etc.) element-by-element. If the vectors are
| of different lengths, R 'recycles' the shorter vector until it is the same length
| as the longer vector.

...

  |=======================================================                    |  74%
| When we did z * 2 + 100 in our earlier example, z was a vector of length 3, but
| technically 2 and 100 are each vectors of length 1.

...

  |=========================================================                  |  76%
| Behind the scenes, R is 'recycling' the 2 to make a vector of 2s and the 100 to
| make a vector of 100s. In other words, when you ask R to compute z * 2 + 100, what
| it really computes is this: z * c(2, 2, 2) + c(100, 100, 100).

...

  |===========================================================                |  79%
| To see another example of how this vector 'recycling' works, try adding c(1, 2, 3,
| 4) and c(0, 10). Don't worry about saving the result in a new variable.

> c(1,2,3,4)+c(0,10)
[1]  1 12  3 14

| You are really on a roll!

  |=============================================================              |  82%
| If the length of the shorter vector does not divide evenly into the length of the
| longer vector, R will still apply the 'recycling' method, but will throw a warning
| to let you know something fishy might be going on.

...

  |===============================================================            |  84%
| Try c(1, 2, 3, 4) + c(0, 10, 100) for an example.

> c(1,2,3,4)+c(0,10,100)
[1]   1  12 103   4
Warning message:
In c(1, 2, 3, 4) + c(0, 10, 100) :
  longer object length is not a multiple of shorter object length

| Great job!

  |=================================================================          |  87%
| Before concluding this lesson, I'd like to show you a couple of time-saving
| tricks.

...

  |===================================================================        |  89%
| Earlier in the lesson, you computed z * 2 + 100. Let's pretend that you made a
| mistake and that you meant to add 1000 instead of 100. You could either re-type
| the expression, or...

...

  |=====================================================================      |  92%
| In many programming environments, the up arrow will cycle through previous
| commands. Try hitting the up arrow on your keyboard until you get to this command
| (z * 2 + 100), then change 100 to 1000 and hit Enter. If the up arrow doesn't work
| for you, just type the corrected command.

> (z*2+1000)
[1] 1002.20 1018.00 1006.28

| Almost! Try again. Or, type info() for more options.

| If your environment does not support the up arrow feature, then just type the
| corrected command to move on.

> z*2+1000
[1] 1002.20 1018.00 1006.28

| Great job!

  |=======================================================================    |  95%
| Finally, let's pretend you'd like to view the contents of a variable that you
| created earlier, but you can't seem to remember if you named it my_div or myDiv.
| You could try both and see what works, or...

...

  |=========================================================================  |  97%
| You can type the first two letters of the variable name, then hit the Tab key
| (possibly more than once). Most programming environments will provide a list of
| variables that you've created that begin with 'my'. This is called auto-completion
| and can be quite handy when you have many variables in your workspace. Give it a
| try. (If auto-completion doesn't work for you, just type my_div and press Enter.)

> my_div
[1] 3.478505 3.181981 2.146460

| Great job!

  |===========================================================================| 100%
| Would you like to receive credit for completing this course on Coursera.org?

1: No
2: Yes

Selection: 2
What is your email address? gargarkwamegideon12@gmail.com
What is your assignment token? 6N9COxV3aLD1mYuh
Grade submission succeeded!

| You got it!

| You've reached the end of this lesson! Returning to the main menu...

| Please choose a course, or type 0 to exit swirl.

