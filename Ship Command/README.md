# Ship Commands
This command will get the user name of the one who uses it and the one who got mentioned by the user.<br>
After nightbot gets the 2 names it will randomly make a ship name.<br>
Of course, the code will remove duplicate letters. It removes the character `VT`, `TTV`, `_` and `0-9`<br><br>

#### Example
![Example](https://i.imgur.com/8jwEGQ2.png)
<br><br><br>

## How to do it:
### In the Pastebin

Make a new Pastebin then put this in your Pastebin
```js
const undup = (str) => [...new Set(str)].join('');
const changer = (str) => str.replace(/\d|vt|VT|_|TTV|ttv| /g, '');
 
const rMention = changer(e).match(/(...?)| /g);
const mRandom = rMention[Math.floor(Math.random() * rMention.length)];
 
const fUser = undup(changer(s)).split('', 3).join('');
const fMention = undup(mRandom).split('').reverse().join('');
 
`${fUser}${fMention}`
```
<br>

### In the [Nightbot Website](https://nightbot.tv)

Add a new command then put in the name
```
!ship
```
Then put in the message this
```
$(user) and $(touser) ship name is "$(eval s=`$(user)`; e=`$(touser)`.toLowerCase(); $(urlfetch PASTEBINLINK))"
```
Just Change the `PASTEBINLINK` into your actual link to get the command working
