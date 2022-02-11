# Maria's Hangman Game -- COPY -- ADD SOUND

#import simple colors module 
from simple_colors import *
#Module includes -- Source [https://pypi.org/project/simple-colors/] 
#Colors: black,red,green,yellow,blue,magenta and cya  n
#Styles: bold, bright,dim,italic,underlined,blink,reverse
def hangManGame():
  hangmanImage = ['''
  +---+
  |   |
      |
      |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
      |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
  |   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
 /|   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
 /|\  |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
 /|\  |
 /    |
      |
=========''', '''
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========''']
 
  # Welcoming statement
  print(magenta("Welcome to my Hangman Game!",["bold"]))
  print()
  nameU = input((blue("What's your name? ", ["italic"])))
  # Asking user if they think they can win, they can say "No" once, if they say yes the first time -- Rules will display--
  correctO = ["Yes","yes","YES","yEs","YeS"]
  nope1 = ["No", "no","NO","nO"]
  for response1 in correctO:
      optionU = input((cyan("YOU think YOU have what it takes? (ง'̀-'́)ง ", ["bright"] )))
      if optionU in correctO:
        print()
        print(yellow("!! ONLY use uppercase from now on !!",["underlined"]))
        print()
        print(green("RULES",["bold","dim","underlined"]))
        print(green("The user, YOU, will have to guess a certain amount of letters to guess a word completely. However you DO NOT have unlimited tries. You will ONLY have a certain amount of tries depending on the word, ranging between 5 to 9 attempts. If you are able to guess 5 letters correctly, I will give you the option to guess the entire word. If you guess the word correctly YOU WIN, if not YOU LOSE. One more thing all words and letters are CAPITALIZED. One last thing the hangman will ONLY display after your failed attempts, and it will show the incorrect letters",["bold"]))
        print()
        print(magenta("We shall begin " + nameU +"!"))
        print()
        print()
        break
      elif optionU in nope1:
        print(red("You have no other option -_- ", ["bold"]))
      else: 
        print("ERROR RESTART, THERE IS NO WAY BACK")

  # Category
  print(cyan("Today's category for the game are basic PC Components!",["blink"]))
  pcList = ["MOTHERBOARD", "PROCESSOR", "STORAGE","MEMORY","COOLING"]
  numOfWords = len(pcList)

  #import random choice from the list 
  from random import choice
  answer = choice(pcList)
  #print(answer) --- Answer will display if hashtags deleted

  #Using length function to display how many letters in the word
  numOfWords = str(len(pcList))
  wordLength = "_" * len(answer)
  print(yellow ("There is a total of " + numOfWords + " words. And each of these words range from 6 - 11 letters."))
  print()

  #number of tries for incorrect and correct guesses
  numTries = 0
  numbTries = 0
  lettersU = []

  print(wordLength)
  #loop 
  while numTries < 9:
    guessUser = input (magenta("Guess a letter: "))
    guessUser.upper()
    if guessUser in answer:
      print(green("Correct"))
      #wwww.append(wordLength) #new addition
      numbTries += 1
      if numbTries >= 5:
        #giving the user option to guess the entire word 
        userOpt1 = input (cyan("Enter code word 'HG' to guess the entire word, if not type 'HJ': "))
        userOpt2 = (magenta("Guess the word:"))
        if userOpt1 == "HG":
          userOpt3 = input(yellow("Guess the entire word:"))
          if userOpt3 == answer:
            print(green("That's the correct word! " + nameU +", You Win!! ｡◕‿◕｡"))
            
            break
          else:
           print(red("Sorry, you didnt guess it right.",nameU, " You Lose ༼ つ ಥ_ಥ ༽つ "))
        elif userOpt1 == "HJ":
          pass
    elif guessUser != answer:
        print(red("The letter is not correct, try again. Make sure you use UPPERCASE ONLY. "))
        numTries += 1 
        print(hangmanImage[numTries])
        print("You've used these letters: :")
        lettersU.append(guessUser)
        print(lettersU)
        #print("Currently the word is: " , wordLength)
    elif numTries == 9:
        
        print(red("Game Over", [bold]))
        break
      
    else:
        print("You have no more attempts", nameU , "play again... 👁👄👁")
hangManGame()
