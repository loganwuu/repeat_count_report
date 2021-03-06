# Word Repeat Counter

##### A Silex app that displays how frequently a word appears in a given string. (8/14/2015)

#### By Logan Wu

## Description
Users input both the word and the string of words to check for the number of full word matches.

## Setup
* Open Terminal
* Enter the web directory in count_repeat folder using terminal
* Enter the following command into terminal 'php -S localhost:8000'
* Open a web browser and type this into the address bar 'localhost:8000'
* Requires Silex/Silex ~1.1 and Twig/Twig ~1.0 to be installed in the count_repeat project folder on the console by typing in "composer install" and then "composer update"

## Technologies Used

PHP, HTML, CSS, Silex, Twig, PHPUnit, Composer

## Specs

1. If user searches for a word that matches the word in a one-word string, it should return 1 repeat.
    * Input: word="dog"; string="dog"
    * Output: "The word 'dog' appears 1 time in 'dog'."

2. If user searches for a word that does not match the word in a one-word string, it should return 0 repeat.
    * Input: word="dog"; string="cat"
    * Output: "The word 'dog' appears 0 time in 'cat'."

3. If user searches for a word that match a word in a multi-word string once, it should return 1 repeat.
    * Input: word="dogs"; string="I love dogs."
    * Output: "The word 'dogs' appears 1 time in 'I love dogs'."

4. If user searches for a word that match a word in a multi-word string twice, it should return 2 repeat.
    * Input: word="dog"; string="I love dog 1 and dog 2."
    * Output: "The word 'dog' appears 2 times in 'I love dog 1 and dog 2'."

5. Uppercase or lowercase letters should not matter.
    * Input: word="DOGS"; string="I love dogs."
    * Output: "The word 'DOGS' appears 1 time in 'I love dogs'."

6. Only alphabetic letters are allowed in the word search box.
    * Input: "0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "`", "~", "!", "@", "#", "$", "%", "^", "&", "*", "(", ")", "_", "+", "-", "=", "{", "}", "|", "\", ":", """, ";", "'", "<", ">", "?", ",", ".", "/"
    * Output: "Sorry, please only enter one word to search for without any space or non-alphabetic characters."

7. If empty entry for the word search box, return "Please enter a word to search for."
    * Input: word=""; string="I love dogs."
    * Output: "Please enter a word to search for."

8. If empty entry for the string search box, return "Please enter a paragraph to search from."
    * Input: word="dog", string=""
    * Output: "Please enter a paragraph to search from."

9. If both fields are empty, return "Please enter a word to search for and a paragraph to search it from."
    * Input: word="", string=""
    * Output: "Please enter a word to search for and a paragraph to search it from."

## Legal

Copyright (c) 2015 **Logan Wu**

This software is licensed under the MIT license.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
