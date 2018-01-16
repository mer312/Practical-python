# Practical-python
#weight example

def isanumber(weight):

    try:
        float(repr(weight))
        bool_weight = True
    except:
        bool_weight = False

    return bool_weight

weight=201
if isanumber(weight): 
    float(weight)       
else:
    print("not a number")
    
if weight <= 200:
            print("skinny")
        elif weight > 200 and weight <= 250:
            print ("moderately fat")
        else: 
            print("you are fat")
            
 def inputNumber(message):
  while True:
    try:
       userInput = int(input(message))       
    except ValueError:
       print("Not an integer! Try again.")
       continue
    else:
       return userInput 
       break 
     

#MAIN PROGRAM STARTS HERE:
weight = inputNumber("How fat are you?")

if weight <= 200:
    print("skinny")
elif weight > 200 and weight <= 250:
    print ("moderately fat")
else: 
    print("you are fat")
