# Game
answer = input("Player1:please insert the number(1-100):")
answer = int(answer)
is_correct = False
try_correct = 0
while try_correct<10 and is_correct == False:
    guess = int(input("player2:please guess a number!"))
    if guess == answer:
        print("player2:You won!")
        is_correct = True
    elif guess > answer:
        print("Your guess is grater than the  answer.")
        try_correct += 1
    else:
        print("Yor guess is smaller than the answer.")
        try_correct += 1
        if is_correct == False:
            print("player2:You lost")


