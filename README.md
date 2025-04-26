Question: Case Conversion for Strings
Write a program that converts a given string such that:

All uppercase characters are converted into lowercase characters.
A hyphen(-) should be present before each uppercase character excluding the first uppercase character.
For Example string = "KeepLearning":

Output:
keep-learing
-----------------------------code-----------------------------------

string = input()
length = len(string)
first_char_lowercase = string[0].lower()

result_string = first_char_lowercase

for index in range(1, length):
    uppercase_char = string[index].upper()
    if string[index] == uppercase_char:
        lowercase_char = string[index].lower()
        result_string = result_string + lowercase_char
    else:
        result_string = result_string + string[index]

print(result_string)
