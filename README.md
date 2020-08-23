# DS-20
## A pangram is a sentence which uses all the letters of the alphabet(a-z)
### example of a pangram: the quick brown fox jumps over the lazy dog.
def pangram(str):
    import string
    small=set(string.ascii_lowercase) #ascii_lowercase contains all the lower case alphabets
    return small<=set(str.lower()) #lower will change all input letters to lower case, set will remove duplicates
s=input('enter string:')
if(pangram(s)):
    print('It is a Pangram')  #if the input string contains all letters this statement will be printed.
else:
    print('It is not a pangram') #if the input string does not contain all the letters this stmt will be printed.
