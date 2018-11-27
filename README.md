# csPortfolio

* WebPage [here](https://maxximusc.github.io/testPage/dogPage2/dogPage.html)
* Lightning [here](https://maxximusc.github.io/lightning2/)
* Lighting JS[here]()
* Dice [here](https://maxximusc.github.io/dice3/)
* Chemotaxis [here](https://maxximusc.github.io/chemotaxis4/)

```Java
if (blockedDot == true) {
      for (int q = 0; q < triggered.length; q++) {
        if (triggeredDot[q] == 1) {
          if (army.get(i).getXpos() - 1 - round(random(army.size())) < objects.get(q).getXpos() - 15) {
            army.get(i).setXpos(j1 - 1 - round(random(army.size())));
          } else if (army.get(i).getXpos() + 1 + round(random(army.size())) > objects.get(q).getXpos() + objects.get(q).getLength() + 15) {
            army.get(i).setXpos(j1 + 1 + round(random(army.size())));
          }
          if (army.get(i).getYpos() - 1 - round(random(army.size())) < objects.get(q).getYpos() - 15) {
            army.get(i).setYpos(j2 - 1 - round(random(army.size())));
          } else if (army.get(i).getYpos() + 1 + round(random(army.size())) > objects.get(q).getYpos() + objects.get(q).getWidth() + 15) {
            army.get(i).setYpos(j2 + 1 + round(random(army.size())));
          }
        }
      }
    }
```
* This code was challenging to write simply because of how precise and specific it had to be in order to function properly. The code above was pulled from my Chemotaxis lab. It basically is checking if a blockade is in the way of a dot so that the dot will be unable to pass through it. It also decides which direction the dot is able to go so that it may get away from the blockade eventually.

* Solving this issue was tough. I had to use booleans as off/on switches, turning them at the right exact moments to make things work out properly. I also found it easier to have an arraylist that would keep track of all the dots that have been blocked (triggered).
