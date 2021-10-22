import random


def password_check(x):

    words = list(x)

    up = 0
    low = 0
    dig = 0

    if len(words) < 6:
        print("Your password is too short. Try again.")
    elif len(words) > 20:
        print("Your password is too long. Try again.")
    for i in words:
        if i.islower() == True:
            low = low + 1
        elif i.isupper() == True:
            up = up + 1
        elif i.isdigit() == True:
            dig = dig + 1

    if up == 0:
        print("Your password is missing an upper case letter. Try again.")
    if low == 0:
        print("Your password is missing a lower case letter. Try again.")
    if dig == 0:
        print("Your password is missing a digit. Try again.")
    if up > 0 and low > 0 and dig > 0:
        print("The password you have entered is valid.")
        
x = input("Please enter a password: ")
password_check(x)


password = []
upcase = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
lowcase = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
size = random.randrange(6,20)

while len(password) <= int(size):
    upp = random.choice(upcase)
    loww = random.choice(lowcase)
    digy = random.randint(0,9)

    password.append(upp)
    password.append(loww)
    password.append(digy)

random.shuffle(password)

final = "".join(str(x) for x in password)



password_creator()

password_check(final)
