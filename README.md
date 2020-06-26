# extracting-date-from-a-file-in-python
import re
string=str(input("enter a string"))
p='[0-9][0-9]{1,2}\/[0-9][0-9]{1,2}\/[0-9][0-9][0-9][0-9]{2,4}'
string.strip()                                 #remove unwanted whitespaces
string =string.split()                         #coverting string into list
for i in string:
  match=re.findall(p,i)                        #returns a list if found
  if match:
    print(match)                               #prints if the date format is found and returns in a list format
