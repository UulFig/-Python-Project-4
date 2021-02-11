# -Python-Project-4
#4 Count to a number(Input) as Loop

def inputNumber(message):
    while True:
        try:
            userInput = int(input(message))
        except ValueError:
            print("Please, put an valid number.\n")
            continue
        else:
            return userInput
            break

number = inputNumber("Choice a number to count. :)\n")

for i in range(int(number)):
    print(i + 1)
