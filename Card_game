#Create a simple Card game in which there are 8 cards which are randomly chosen from a deck. 
#The first card is shown face up. The game asks the player to predict whether the next card in the selection will have a 
#higher or lower value than the currently showing card.
#For example, say the card that’s shown is a 3. The player chooses “higher,” and the next card is shown. 
#If that card has a higher value, the player is correct. In this example, if the player had chosen “lower,” 
#they would have been incorrect. If the player guesses correctly, they get 20 points. 
#If they choose incorrectly, they lose 15 points. If the next card to be turned over has the same value as the previous card, 
#the player is incorrect.

class Card:
    values=[None,None,2,3,4,5,6,7,8,9]  

from random import shuffle
class Deck(Card):
    def __init__(self):
        self.cards = []
        for i in range(2, 10):
                self.cards\
                    .append(i)        
        shuffle(self.cards)     #shuffling the cards

    def rm_card(self):
        if len(self.cards) == 0:
            return
        return self.cards.pop() #showing random face card
        
    
class Game(Deck):
    def player(self,x):
        self.x=x
        while x=="Higher":
            face=cgame.rm_card() #not sure if this is the correct way
            n=0
            for n in self.cards:
                if n>face:
                    print("Correct:You gain 20 points")
                elif n<face:
                    print("Incorrect:You lose 15 points")
                else:
                    print("Incorrect:The card values are equal")
                break
            
            
class Points(Game):
    def total(self,x):
        t=0
        if (x=="Higher"and n>face) and (x=="Lower" and n<face):
            t+=20
        elif (x=="Higher"and n<face) and (x=="Lower" and n>face):
            t-=15
        else:
            pass
        print(f"Total:{t}")

            
cgame=Points()
print(cgame.rm_card())
print(cgame.player("Higher"))
cgame.total("Higher") #total points are not being shown
