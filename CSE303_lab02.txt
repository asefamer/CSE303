#CSE303_lab02
#2018-2-60-068

#In[1]:

#1. find all the number from 1-1000 that are divisible by 8

nums=[1 for i in range(1,1001)if (i%8)==0]
print('Result list:',nums)

#In[2]:

#2.Find all of the numbers from 1-1000 that have a 6 in them

nums=[i for i in range(1,1001)if '6'in str(i)]
print('Result list:',nums)


#In[3]:

#Count the number of spaces in a string(use string above)

string="practice Problem to Dril list Comprehension in your Head."
print('Print spaces Count:',string.count(''))


#In[4]:
#4.Remove all the vowels in a string(use string above)

string="Practice Problem to Drill list Comprehension in your Head."
vowel="aeiouAEIOU"
print("".join([char for char in string if char not in vowel]))


#In[5]:

#5.Find all of the words in a string that are less than 5 latters(use string above)

string="Practice Problem to Drill list Comprehension in your head."

words=[x for x in string.split(' ')]
new_word=[word for word in words if(len(word)<5)]
print(new_word)

#In[6]:
#6.Use a dictionary comprehension to count the lenght of each word in a sentence(use string above)

string="Practice Problems To Drill list Comprehension in your Head."
li=string.split(' ')

d={word: len(word)for word in li}
print(d)

#In[7]:

#7. Usa a nested list comprehension to find all of the numbers from 1-1000 that are divible by any
#single digit beside 1(2-9)

numbers =[i for i in range(1,1001) if(True) in [True for j in range(2,10) if(i%j ==0)]]
print(numbers)

# In[8]:

#8.For all the numbers 1-1000,use a nested list/dictionary comphension to find the highest single
#digit any of the numbers is divisible by

numbers={i:max([j for j in range(1,10) if i%j==0])for i in range(1,1001)}
print(numbers)

#In[]:
               


