# Guessing_Game
 Guessing_Game - It's a project to learn programming

from random import randint
from time import sleep

print(70*'=')
print('\033[35mI am thinking about a random number between \033[32m1 and 10\033[m ... \033[35mTry to guess!\033[m ')
print(70*'=')

pc = randint(1, 10)
human = 0

human = int(input('Type the number that i am thinking: '))
print('\033[33m Processing\033[m...')
sleep(1.5)

while human != pc:
    human = int(input('\033[31mOh... you missed\033[m, \033[33mtry again my friend\033[m! Type another number: '))
    print('\033[33m Processing\033[m...')
    sleep(1)


if human == pc:
    print('\033[32mCongratulations\033[m, you are\033[32m right\033[m!!')
