import random
n = random.randint(4,31)
print("Число камней в куче: ",n)
while n > 0:
    us = int(input("Сколько камней возьмём?"))
    if us<=0 or us>3:
        print("возьмите от 3 до 4 камней")
        exit()
    n -= us
    print("Камней в куче: ",n)
    if n == 1:
        print("ПОБЕДА!")
        exit()
    n - random.randint(1,4)
    print("Камней в куче после хода соперника: ", n)
    if n == 1:
        print("ПОРАЖЕНИЕ((")
        exit()

