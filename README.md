# Practical-python
#weight example

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
