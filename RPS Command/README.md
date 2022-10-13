# RPS(Rock, Paper, Scissors) Command
This command will let you play with nightbot in a Rock Paper Scissors Game.

#### Example
![Example](https://i.imgur.com/DndmMUt.png)
<br><br><br>

## How to do it:
### In the Pastebin

Make a new Pastebin then put this in your Pastebin
```txt
:[rock] $(sender) chose ⛰, Nightbot chose 📜 -- Better luck next time.
:[rock] $(sender) and Nightbot both chose ⛰. -- It’s a tie… yuck!
:[rock] $(sender) chose ⛰, Nightbot chose ✂️. -- $(sender) wins! PogChamp
:[paper] $(sender) chose 📜, Nightbot chose ✂️. -- Better luck next time.
:[paper] $(sender) and Nightbot both chose 📜. -- It’s a tie… yuck!
:[paper] $(sender) chose 📜, Nightbot chose ⛰. -- $(sender) wins! PogChamp
:[scissors] $(sender) chose ✂️, Nightbot chose ⛰. -- Better luck next time.
:[scissors] $(sender) and Nightbot both chose ✂️. -- It’s a tie… yuck!
:[scissors] $(sender) chose ✂️, Nightbot chose 📜. -- $(sender) wins! PogChamp
$(sender),  Are you going to shoot or what? I can’t play ⛰📜✂️ by myself...
```
<br>

### In the [Nightbot Website](https://nightbot.tv)

Add a new command then put in the name
```
!rps
```
Then put in the message this
```
$(urlfetch https://api.thefyrewire.com/twitch/pastebin/PASTEBINCODE?filter=$(1)&user=$(user))
```
Just Change the `PASTEBINCODE` to your pastebin code. You will see your code after creating your pastebin.<br>
Example is `pastebin.com/wwvdjvEj` just get the `wwvdjvEj` and that is your pastebin code
