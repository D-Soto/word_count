# word_count
Check the number of each word in a story
Text = """Text_File"""
for pun in '-.,\:;"!()':
    Text = Text.replace(pun,' ')
Text = Text.lower()
#print(Text)
word_list = Text.split()
#print(word_list)
d= dict()
for w in word_list:
    d[w] = d.get(w,0) + 1
print(d)
