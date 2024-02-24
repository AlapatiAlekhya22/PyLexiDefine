# PyLexiDefine
PyLexiDefine is a Python-based English Dictionary application designed to provide users with quick and comprehensive definitions of English words. This project utilizes Python programming skills along with data structures such as dictionaries.
import json

print('*****Welcome to the Dictionary App*****')
print('Please select your choice:')
print('1. Add a word into dictionary')
print('2. Find the meaning of word')
print('3. Update the word to dictonary')
print('4. Exit')


s = open('word.txt','w')
coll_word = {}
json.dump(coll_word,s)
s.close()

while True:
num = int(input('Enter the Choice:'))
if num == 1:
import json
s = open('word.txt','w')
d = input('Enter a word : ')
wm = input('Enter the meaning of word : ')
coll_word[d] = wm
json.dump(coll_word,s)
s.close()

elif num == 2:
import json
s = open('word.txt','r+')
app = json.load(s)
search = input('Enter the word to search: ')
if search in coll_word:
print('The meaning of word',search, ' is',coll_word.get(find))
else:
print('word not found enter again or add word ')
json.dump(coll_word,s)
s.close()
elif num == 3:
import json
s = open('words.txt','w')
d1 = input('Enter the word:')
upm = input('Enter the updated meaning: ')
coll_word[d1] = upm
json.dump(coll_word,s)
s.close()
elif num == 4:
print('********Thank you for choosing Dictionary app**********')
print("********GOOD BYE HAVE A NICE DAY*********")
break
else:
print('Enter the correct choice given below')
print('1. Add ')
print('2. Find the meaning of word')
print('3. Update the meaning of word')
print('4. Exit')
