# Networks-Project1

This is my first project for my Networks & Distributed Systems course. 

The assignment description is below:

This assignment is intended to familiarize you with writing simple network code. You will implement a client program that plays a variant of the recently popular game Wordle. Your program will make guesses for the secret word, and the server will give you information about how close your guess is. Once your client correctly guesses the word, the server will return a secret flag that is unique for each student. If you receive the secret flag, then you know that your program has run successfully.

Your client must support TLS encrypted sockets. The server will return different secret flags depending on whether your client communicates with or without TLS. To receive full credit on this project, you must turn in both secret flags: the one retrieved via a non-encrypted socket, and the one retrieved via a TLS encrypted socket.

Approach:
My approach to this project was to go to office hours and learn how to break down the problem and gain a better understanding of how to begin writing this assignment because I had little to no understanding of how to do the first step - create a connection to the server. I  decided to write in Python as I want to expand my skillset and future starter code will be in Python. After learning which libraries to utilize, I researched the argparse, python, ssl, json, and python documentation. From there I continued to struggle and went to more office hours, where I better understood unix commandline. From there I was able to go forth with the project in creating connections to the server, sockets, and sending data to the server to finish the Wordle game.

Challenges:
- Learning how to create a connection to the socket
- Learning how to create a socket
- Encoding and Decoding sending and receiving data from both a TLS and TCP server
- Creating the Wordle search algorithm to skip words

Guessing Strategy:
I began my Wordle guess with the word 'salet,' after which I wrote a method that would take the values from the most recent marks array that was returned. The method would input correct letters (outputs of 1) into an array with no duplication, and perfect letters (outputs of 2) into an array in the index it was found at. Thus keeping track of letters that are in the word, and letters found that were in the word and in the right place. Then I looped through all possible words, skipping words that did not contain all correct letters, and words that did not contain the correct letters in the right place.

Testing Strategy:
I tested my code through running the code and printing out the values of what was outputted from the server. I also increased my scrollback line length in order to be able to compare results and then look for what went wrong. I also tested through running the code over and over to ensure consistent results, and submitting it to the Gradescope autograder.