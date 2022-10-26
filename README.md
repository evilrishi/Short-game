# Short-game
import random
def gamewin(comp,you):
    if comp==you:
        return None
    elif comp=='R':
        if you=='S':
            return False
        elif you=='P':
            return True
    elif comp=='P':
        if you=='R':
            return False
        elif you=='S':
            return True
    elif comp=='S':
        if you=='P':
            return False
        elif you=='R':
            return True
print("comp turn:Rock(R) Paper(P) Scisors(S)")
randNO=random.randint(1,3)
if randNO==1:
    comp='R'
elif randNO==2:
    comp='P'
elif randNO==3:
    comp='S'
you=input("your turn:Rock(R) Paper(P) Scisors(s) ?")
a=gamewin(comp,you)
print(f"computer choose {comp}")
print(f"you choose {you}")
if a==None:
    print("the game is tie")
elif a:
    print("you win")
    



        
