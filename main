from random import *

letterList = ["x","y","a","b","k","m","n","z","c","x","y","a","b","k","m","n","z","c"]

class Var:

    def __init__(self,letter):
        self.number = randint(1,20)
        self.letter = letter
        self.sign = choice(["+","-","+","-","+","-","+","-","+","-","+","-"])

    def __str__(self):
        if self.letter == "":
            if self.sign == "-":
                return f" - {self.number}"
            else:
                return f" + {self.number}"
        elif self.number == 1:
            if self.sign == "-":
                return f" - {self.letter}"
            else:
                return f" + {self.letter}"
        else:
            if self.sign == "-":
                return f" - {self.number}{self.letter}"
            else:
                return f" + {self.number}{self.letter}"

class Question:

    def __init__(self,lettersNumber,varsNumber):
        self.letters = [""]
        self.vars = []
        for a in range(lettersNumber):
            self.letters.append(choice(letterList))
        for a in range(varsNumber):
            self.vars.append(Var(choice(self.letters)))

    def __str__(self):
        t = ""
        for i in self.vars:
            t += f"{i}"
        return t


n=10
for x in range(n):
    print(Question(2,10))
