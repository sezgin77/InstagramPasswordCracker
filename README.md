# InstagramPasswordCracker
Takes an argument of a username and a password list from standard input. Brute forces instagram account based on provided password list.

This program uses the library known splinter to interact with the instagram website. This library is well documented and has few dependencies.

You must have firefox installed, or if you use google chrome all you have to do is change "with Browser('firefox', headless=True)" to "with Browser('chrome', headless=True)". Simple as that.

Instagram gives a timeout of about 11 mins after 14 to 25 invalid passwords are tested. The program will wait for that time when it gets a certain error message before attempting to crack again.

On average, the program will be able to test around 60 to 125 passwords in an hour.

The slow speeds are due to the timeout and not the fact that this program is written in Python.

This code is intended for educational purposes. Please DO NOT use this program for malicious purposes.

The password list file provided must seperate passwords with a newline.

Usage:

./insta_cracker [username] < [password list file]