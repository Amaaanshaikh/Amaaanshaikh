I have just started learning python, here is what I do, 
Starting with comments,
Adding notes in the program is known as comments, and they start with symbol #
# to compute the percentage of the hour that has elapsed
# percentage = (minute*100)/60
# print(percentage)
# Debugging, There are 3 kinds of debugging, syntax errors, runtime errors, and semantic error.
# Syntax error, refers to the structure of a program and the rules about that structure.
# Runtime error, The second error, its known as runtime error because the error does not appear until after the program has started running. These errors are known as exceptions because they usually indicate that something exceptional(and bad) has happened.
# Semantic error, The third type of error is "semantic", which means related to meaning. If there is a semantic error in your program, it will run without generating error message, but it will not do the right thing. It will do something else. Specifically, it will do what you told it to do.
# Glossary of the output,
# 1 Variable - A name that refers to a value.
# 2 Assignment - A statement that assigns a value to a variable
# 3 State Diagram - A graphical representation of a set of variables and the value they refer to.
# 4 Keyword - A reserved word that is used to parse a program; you cannot use keywords like, if, def and while as variables names.
# 5 Operand - one of the values on which an operator operates.
# 6 Expression - A combination of variable 
# 7 Evaluate - To simplify an expression by performing the operations order to yield a single value.
# 8 Statement - A section of code that represents a command or action. So far, the statements we have seen are assignments and print statements.
# 9 Execute - To run a statement and do what it says.
# 10 Interactive mode - A way of using the python interpreter by typing code at the prompt.
# 11 Script mode - A way of using the python interpreter to read code from a script and run it.
# 12 Script - A program stored in a file.
# 13 Order of operations - Rules governing the order in which expressions involving multiple operators and operands are evaluated.
# 14 Concatenate - To join two operands end-to-end.
# 15 Comment - Information in a program that is meant for other programmers (or anyone reading the source code) and has no effect on the execution of the program. 
# 16 Syntax error - An error in a program that makes it impossible to erase (and therefore impossible to interpret)
# 17 - Exception - An error in a program that makes it impossible to detect until the program is ran. 
# 18 - Semantic error - A type of error that is not possible to detect, does exactly the same but something other than what the programmer intended.
# 19 Now I'm learning Naming rules and conventions,
# 20 Names cannot contain spaces
# 21 Names may be a mixture of upper and lower case characters
# 22 Names can't start with a number but may contain numbers after the first character 
# 23 Variable names and functions names should he written in snake_case, which means that all letters are lowercase and words are seperated using undersocre.
# 24 Descriptive names are better than cryptic abbreviations because they help other programmers read and interpret your code. For example, student_name is better than sn. It may feel excessive when you write it, but when you return to your code you'll find it much easier to understand.

# with the help of google colab I made a program, where you guess the number game.
import random

def guess_the_number():
    while True: # Outer loop for playing multiple rounds
        secret_number = random.randint(1, 100)
        guess = 0
        attempts = 0

        print("\nWelcome to Guess the Number!")
        print("I'm thinking of a number between 1 and 100.")

        while guess != secret_number:
            try:
                guess = int(input("Take a guess: "))
                attempts += 1

                if guess < secret_number:
                    print("Too low! Try again.")
                elif guess > secret_number:
                    print("Too high! Try again.")
                else:
                    print(f"Congratulations! You guessed the number in {attempts} attempts!")
            except ValueError:
                print("Invalid input. Please enter a whole number.")

        play_again = input("Do you want to play again? (yes/no): ").lower()
        if play_again != 'yes':
            print("Thanks for playing!")
            break # Exit the outer loop if the user doesn't want to play again

# In this after running the program, you need to guess a number and the program will tell the frequency in what the number is valid in, for example, if the number is higher, it will say "Too High", if the number is low, it will say "Too Low" and if the number is correct it will say Congratulations! You guessed the number in {attempts} attempts! and the attempts in the bracket shows the number of tries.

# Tim Peters, A python programmer, wrote this,
# The Zen of Python,
# Beautiful is better than ugly.
# Explicit is better than implicit.
# Simple is better than complex.
# Complex is better than complicated.
# Flat is better than nested.
# Sparse is better than dense.
# Readability counts.
# Special case aren't special enough to break the rules.
# Although practically beats purity.
# Errors should never pass silently.
# Unless explicitly silenced.
# In the face of ambiguity, refuse the temptation to guess.
# There should be one–and preferably only one–obvious ways to do it.
# Although that way may not be obvious at first unless you're dutch.
# Now is better than never.
# Although never is often better than *right* now.
# If the implementation is hard to explain, it's a bad idea.
# If the implementation is easy to explain, it's may be a good idea.
# Namespaces are one honking great idea -- let's do more of those.

# Now we will review Data types
