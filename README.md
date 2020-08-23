# Pangram
## A pangram is a sentence which uses all the letters of the alphabet(a-z)
### example of a pangram: the quick brown fox jumps over the lazy dog.
def pangram(str):
	import string
	x=set(string.ascii_lowercase) #ascii_lowercase gives all the lower case alphabets
	return x<=set(str.lower()) #lower will change all input letters to lower case, set will remove duplicates
s=input('enter string:')
if(pangram(s)):
	print('Given string is a pangram') #if the input string contains all the letters this statement will be printed.
else:
	print('Given string is not a pangram') #if the input string does not contain all the letters this stmt will be printed.
