# Dubrico_2ECE-A - PA #1 (V2)

# 1.) ALPHABET SOUP PROBLEM: Create a function that takes a string and returns a string with its letters in alphabetical order.

**The problem asks for a function that takes a string and returns a new string containing the same letters, but arranged in alphabetical (ascending) order. Thus, it is needed to decide on how to handle case (uppercase vs lowercase) and whether to keep or remove non-letter characters. The core idea is to extract the letters, sort them, and then join them back into a single string.**

    def alphabet_soup(input): # Defines the function

    letters = sorted(input.lower()) # Converts the input string to lowercase and sort the letters

    return ''.join(letters) # Joins the sorted letters back into a string

    input_string = input("Enter a string: ") # Asks for user's input
    result = alphabet_soup(input_string) # Gets the result
    print("Sorted letters:", result) # Displays the output


# 2.) EMOTICON PROBLEM: Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon:

# Smile - :) Grin - :D Sad - :(( Mad - <:(

**The problem asks for a function that takes a sentence and replaces certain keywords with corresponding emoticons. Specifically, replace the words smile, grin, sad, and mad with :) , :D , :(( , and <:( respectively. Thus, it is needed to create a dictionary, split the sentence into words, replace them with emoticons, and join them back again in the sentence.**

    def emotes(sentence): # Defines the function

    emoticons = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": "<:("
    } # Defines a dictionary mapping words to emoticons, with "smile" as ":)", "grin" as ":D", "sad" as ":((", and "mad" as "<:("
    
    words = sentence.split() # Splits the sentence into words
    replaced_words = [emoticons.get(word, word) for word in words] # Replaces words with emoticons
    return ' '.join(replaced_words) # Joins the words back into a sentence

    user_input = input("Enter a sentence: ") # Asks for user's input
    result = emotes(user_input) # Gets the result
    print("Emoticon version:", result) # Displays the output


# 3.) UNPACKING LIST PROBLEM: Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

**The problem asks to split a given list named writeyourcodehere into three variables: first, middle, and last. The first element goes to first, the last element goes to last, and everything in between becomes the list assigned to middle; then all three variables are printed.**

    num = [1, 2, 3, 4, 5, 6] # Make the list
    
    first, *middle, last = num # Declare the variables
    
    Using print() function
    print("first:", first)
    print("middle:", middle)
    print("last:", last) # Print the three variables

--VERSION 2--
