# Ship Commands
In this command it will get the user's name of the one who uses it and the one who got mention by the user.<br>
After nightbot got the 2 names it will randomly make a ship name.<br>
Of course the code will remove duplicate.<br><br>

#### Example
![Example](https://i.imgur.com/8jwEGQ2.png)
<br><br><br>

## How to do it:

Make a new pastebin then put this in your pastebin
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
After making the pastebin 
