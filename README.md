# blackjack
def coins():
    print("Insert the number of players that would like to play")
    players = int(input())
    print("We're starting the game insert the value that you want to play with: ")
    money = int(input())
    credits = money * 100
    print("You have {} coins for each player which is {}".format(credits,players))
def cards():
    import random

    deck = {}
    suits = [{"name":"Hearts"},{"name":"Diamonds"},{"name":"Spades"},{"name":"Clubs"}]
    numbers = [{"name":"2"},{"name":"3"},{"name":"4"},{"name":"5"},{"name":"6"},
               {"name":"7"},{"name":"8"},{"name":"9"},{"name":"10"},{"name":"J"},{"name":"Q"},{"name":"K"},{"name":"A"}]
    for each in numbers:
        deck["numbers"] = each["name"]
    for each in suits:
        deck["suits"] = each["name"]
    randomsuits = random.sample(suits, 1)[0]
    randomnumber = random.sample(numbers,1)[0]
    print(randomsuits, randomnumber)
    
def game():
  
 
coins()
game()
cards()
