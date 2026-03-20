import random
number =random.randint(1,10)
attempts = 0

while True:
 
 guess = int(input("Choose a number btw 1 to 10:"))
 attempts += 1
 if guess==number:
  print("Congratulations🎉")
  print("YOU GUESSEd  IN",attempts,"attempts")
  
  break
 elif guess<number:
  print("TOO LOW")
 else:
  print("TOO HIGH")
 if attempts==5:
  print("GAME OVER😢")
  print("The correct number was", number)
  break