# Ship Commands
This command will show the user their fortune just like a fortune cookie.<br><br>

#### Example
![Example](https://i.imgur.com/STL0Qru.png)
<br><br><br>

## How to do it:
### In the [Nightbot Website](https://nightbot.tv)

Add a new command then put in the name
```
!fortune
```
Then put in the message this
```
Your fortune is "$(eval $(urlfetch https://fortuneapi.herokuapp.com/fortunes).replace('\n', ''))"
```

> This time we don't need Pastebin for the command
