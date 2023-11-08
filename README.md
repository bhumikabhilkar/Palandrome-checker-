# Palandrome-checker-

def is_palindrome(input_string):
    # Remove spaces and convert to lowercase for case-insensitive palindrome check
    input_string = input_string.replace(" ", "").lower()
    # Compare the original string with its reverse
    return input_string == input_string[::-1]

# Get user input
user_input = input("Enter a word or phrase: ")

if is_palindrome(user_input):
    print(f"{user_input} is a palindrome.")
else:
    print(f"{user_input} is not a palindrome.")