# Maria's Hangman Game
def hangManGame():
  # Welcoming statement
  print("Welcome to my Hangman Game!")
  print()
  nameU = input("What's your name? ")
  # Asking user if they think they can win, they can say "No" once, if they say yes the first time -- Rules will display--
  correctO = ["Yes","yes","YES","yEs","YeS"]
  nope1 = ["No", "no","NO","nO"]
  for response1 in correctO:
      optionU = input("YOU think YOU have what it takes? (ง'̀-'́)ง " )
      if optionU in correctO:
        print()
        print("!! ONLY use uppercase from now on !!")
        print()
        print("RULES")
        print("The user, YOU, will have to guess a certain amount of letters to guess a word completely. However you DO NOT have unlimited tries. You will ONLY have a certain amount of tries depending on the word, ranging between 5 to 9 attempts. If you are able to guess 5 letters correctly, I will give you the option to guess the entire word. If you guess the word correctly YOU WIN, if not YOU LOSE. One more thing all words and letters are CAPITALIZED.")
        print()
        print("We shall begin",nameU, "!")
        print()
        print()
        break
      elif optionU in nope1:
        print("You have no other option -_- ")
      else:
        print("ERROR RESTART")

  # Category
  print("Today's category for the game are basic PC Components!")
  pcList = ["MOTHERBOARD", "PROCESSOR", "STORAGE","MEMORY","COOLING"]
  numOfWords = len(pcList)
  #import random choice from the list 
  from random import choice
  answer = choice(pcList)
  #Using length function to display how many letters in the word
  numOfWords = len(pcList)
  wordLength = "_" * len(answer)
  print("There is a total of" , numOfWords, "words.")
  print()

  #number of tries for incorrect and correct guesses
  numTries = 0
  numbTries = 0
  print(wordLength)
  #loop 
  while numTries < 9:
    guessUser = input ("Guess a letter: ")
    if guessUser in answer:
      print("Correct") 
      numbTries += 1
      if numbTries >= 5:
        #giving the user option to guess the entire word 
        userOpt1 = input ("Enter code word 'HG' to guess the entire word, if not type 'HJ': ")
        userOpt2 = ("Guess the word:")
        if userOpt1 == "HG":
          userOpt3 = input("Guess the entire word:")
          if userOpt3 == answer:
            print("That's the correct word!" ,nameU,"You Win!! ｡◕‿◕｡")
            
            break
          else:
           print("Sorry, you didnt guess it right.",nameU, " You Lose ༼ つ ಥ_ಥ ༽つ ")
        elif userOpt1 == "HJ":
          pass
    elif guessUser != answer:
        print("The letter is not correct, try again")
        numTries += 1 
    elif numTries == 9:
        print("Game Over")
        break
      
    else:
        print("You have no more attempts", nameU, "play again... 👁👄👁")
hangManGame()
