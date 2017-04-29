# Cipher

A Drupal website showcasing a custom module to encrypt inputted text using the shift/Caesar cipher! 

## Prerequisites

You will need the following things properly installed on your computer.

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [MAMP](https://www.mamp.info/en/)
* [PHP 5.2.5 or higher](http://www.php.net/)

## Installation

**Step 1**: Clone this repository to your local computer

```console
git clone https://github.com/brynnacodes/drupal-cipher
```

**Step 2**: Open MAMP and set the web server document root to the project directory

**Step 3**: Start the Apache and MySQL servers

**Step 4**: Navigate to localhost:8888/phpMyAdmin and import the bookstore.sql.zip file into a database with the same name.

**Step 5**: Visit the website at [http://localhost:8888](http://localhost:8888).

## Planning
* Custom module should present a custom form with 3 text inputs.
* One input should be a shift value, one should be a direction, and the third should be the phrase to be encrypted.
* Redirect to a second page to show the result - the encoded phrase.
* The shift value is the number of places to shift each letter over.
* If the shift direction is "right" then you will add the shift value. For example: "a" with a shift value of 1 and a direction of right would become "b". A shift direction of "left" with a shift value of 1 would turn "b" into "a".
* If the shift amount takes you over the bounds of the alphabet then cycle back to the beginning. For example: a shift value of 3 with the direction of right would turn "z" into "c".
* Any spaces or punctuation in the input phrase should be ignored and reproduced in the final result without being shifted.
* Your final result should be in all lowercase.
* The shift value must be a positive integer
* The shift direction must be either "left" or "right".
* The only special characters that should be allowed in your input phrase are spaces and punctuation.

## Specs
```
1. Input:
Shift value = 3
Shift direction = right
Phrase = "hello"

Output:
"khoor"

2. Input:
Shift value = 1
Shift direction = left
Phrase = "hi there!"

Output:
"gh sgdqd!"

```

## License

Copyright 2017 Brynna Klamkin-McCarter - MIT License
