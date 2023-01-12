# Networks-Project1

This is my first project for my Networks & Distributed Systems course. 

The assignment description is below:

This assignment is intended to familiarize you with writing simple network code. You will implement a client program that plays a variant of the recently popular game Wordle. Your program will make guesses for the secret word, and the server will give you information about how close your guess is. Once your client correctly guesses the word, the server will return a secret flag that is unique for each student. If you receive the secret flag, then you know that your program has run successfully.

Your client must support TLS encrypted sockets. The server will return different secret flags depending on whether your client communicates with or without TLS. To receive full credit on this project, you must turn in both secret flags: the one retrieved via a non-encrypted socket, and the one retrieved via a TLS encrypted socket.


