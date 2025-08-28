# Dubrico_ECE2112 [PA #1]

# 1.) ALPHABET SOUP PROBLEM: Create a function that takes a string and returns a string with its letters in alphabetical order.

    Creating the function
    def alphabet_soup(input): # Define the function

    Using sort function
    letters = sorted(input.lower()) # Convert the input string to lowercase and sort the letters

    Using join() method
    return ''.join(letters) # Join the sorted letters back into a string

    Using input() function
    input_string = input("Enter a string: ") # Ask for user's input
    result = alphabet_soup(input_string) # Getting the result

    Using print() function
    print("Sorted letters:", result) # Print the output


# 2.) EMOTICON PROBLEM: Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon:

Smile - :) Grin - :D Sad - :(( Mad - <:(

    Creating the function
    def emotes(sentence): # Define the function

    Using the dictionary
    emoticons = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": "<:("
    } # Define a dictionary mapping words to emoticons
    
    Using split() method
    words = sentence.split() # Split the sentence into words
    replaced_words = [emoticons.get(word, word) for word in words] # Replace words with emoticons
    return ' '.join(replaced_words) # Join the words back into a sentence

    Using input() function
    user_input = input("Enter a sentence: ") # Ask for user's input
    result = emotes(user_input) # Getting the result

    Using print() function
    print("Emoticon version:", result) # Print the output


# 3.) UNPACKING LIST PROBLEM: Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

    Using the list
    num = [1, 2, 3, 4, 5, 6] # Make the list
    
    first, *middle, last = num # Declare the variables
    
    Using print() function
    print("first:", first)
    print("middle:", middle)
    print("last:", last) # Print the three variables


# 3.) UNPACKING LIST PROBLEM: Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.
