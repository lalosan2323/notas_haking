
## DESCRIPTION
Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_atlas/18/challenge.zip)

## HINT
Have you ever played hot or cold? Binary search is a bit like that.

## SOLUTION

````
- La solución fue ir buscando en mitades hasta encontrar el número correcto. 



EduardoSanchez-picoctf@webshell:~$ ssh -p 64181 ctf-player@atlas.picoctf.net
ctf-player@atlas.picoctf.net's password: 
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 500
Lower! Try again.
Enter your guess: 250
Lower! Try again.
Enter your guess: 125
Lower! Try again.
Enter your guess: 100
Lower! Try again.
Enter your guess: 50
Lower! Try again.
Enter your guess: 20
Higher! Try again.
Enter your guess: 30
Lower! Try again.
Enter your guess: 25
Higher! Try again.
Enter your guess: 27
Congratulations! You guessed the correct number: 27
Here's your flag: picoCTF{g00d_gu355_2e90d29b}

```
