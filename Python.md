# Introduction to Python Scripts

### What's your name
--------------------------------------------
```python
name = raw_input("What is your name?\n")
print("Hi there, " + name)
```

### Average Calculator
--------------------------------------------
```python
print "Welcome to the TIU Average Calculator.. \n"
one = raw_input("Please enter your first reading .. \n")
two = raw_input("Please enter your second reading .. \n")
three = raw_input("Please enter your third reading .. \n")
av = (int(one) + int(two) + int(three))/3
print " ---------------------------- "
print "Your average is .. " + str(av)
print "\n Have a Ducky Day .. \n"
print " ---------------------------- "
```

### Ada Poetry 
```python 
#!/usr/bin/python
import random
print "Hello my name is Ada"
yourname = raw_input("What is your name")
print "Hello ", yourname
print "Click the z key to genearate a poem"
print "Here is your poem ", yourname
verbs = ["laugh","dance","burp"]
adverbs = ["loudly","silently","endlessly"]
nouns =  ["sea","moon","tree"]
adjectives = ["happy","tired","hungry"]
#https://docs.python.org/2/library/random.html
print "I ", verbs[random.randint(0,len(verbs))]
print adverbs[random.randint(0,len(adverbs))]
print "by the ", nouns[random.randint(0,len(nouns))]
print "I feel ", adjectives[random.randint(0,len(adjectives))]
```

### Mash Game 
```python
import random
# Define the M.A.S.H parameters
mash = ('Mansion','Apartment','Shack','Home')

# Create the prompts
mash_prompts = ('List 4 names of individuals you would like to marry.\n',
'List the number of kids you will have (4 values).\n',
'List 4 jobs you would like to have.\n',
'List 4 salaries you hope to have.\n',
'List 4 cars you hope to own.\n',
'List 4 places you would like to live.\n')

# Set the delimiter
delimiter=','
# Ask the questions
print "For each prompt, list 4 items separated by a comma.\n"
smarry = raw_input(mash_prompts[0])
skids = raw_input(mash_prompts[1])
sjobs = raw_input(mash_prompts[2])
ssalaries = raw_input(mash_prompts[3])
scars = raw_input(mash_prompts[4])
splaces = raw_input(mash_prompts[5])

# split the inputted values into an array
lmarry = smarry.split(delimiter)
lkids = skids.split(delimiter)
ljob = sjobs.split(delimiter)
lsalaries  = ssalaries.split(delimiter)
lcars = scars.split(delimiter)
lspaces  = splaces.split(delimiter)

# ranomize values
x = random.randint(0,3)
m = random.randint(0,3)
j = random.randint(0,3)
k = random.randint(0,3)
c = random.randint(0,3)
s = random.randint(0,3)
p = random.randint(0,3)

# strip  --> string.strip(x)
print "Your fortune.. "
print "You will dwell in a " + mash[x]
print "Marred to " + lmarry[m]
print "with " + lkids[k] + " kids"
print "working as a " + ljob[j]
print "making a salary of " + lsalaries[s]
print "driving a " + lcars[c]
print "living in " + lspaces[p]
```


### Turtles
--------------------------------------------
#### Hexagon
```python
import turtle
t = turtle.Pen()
for x in range(1,8):
	t.forward(100)
	t.rt(60)
	t.forward(100)
t.reset()
```	
#### Hexagon Simplified 
```python
----------------------
import turtle
t = turtle.Pen()
for x in range(6):
	t.circle(100)
	t.left(60) 
```
	
--------------------------------------------
Something Cool
import turtle
t = turtle.Pen()
c = ["red","yellow","blue", "green"]
for x in range(100):
	t.pencolor(c[x%4])
	t.forward(x)
	t.left(91)
	
Something Cooler
import turtle
turtle.bgcolor("black")
t = turtle.Pen()
c = ["red","yellow","blue", "green"]
for x in range(100):
	t.pencolor(c[x%4])
	t.forward(x)
	t.left(91)
	

	
