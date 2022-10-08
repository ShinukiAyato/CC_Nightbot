# Shoutout Command
Shoutout command is the most basic command you can do but in here we will make it more advance or detailed.<br>
We are gonna make it so that Nightbot will send different messages when they are live or offline.<br>
Of course I will put in here too the basic shoutout command.<br><br>

#### Example in Basic Shoutout
![Example](https://i.imgur.com/yQAzAyk.png)
<br><br>

#### Example in Advance Shoutout
![Example](https://i.imgur.com/nP8X0Sd.png)
<br><br><br>

## Basic Shoutout
### In the [Nightbot Website](https://nightbot.tv)

Add a new command then put in the name
```
!shoutout
```
Then put in the message this
```
Go check out $(touser), $(twitch $(touser) "they last played {{game}}") at https://twitch.tv/$(touser) !
```
<br><br>
## Advance Shoutout
### In the Pastebin

Make a new Pastebin then put this in your Pastebin
```js
if(s == "live"){
    `${m} is currently LIVE for ${t} now! They are playing ${g}, You can go check them out in ${u}`
} else if(s == "offline"){
    `${m} was last seen playing ${g}. Go check them out in ${u}`
} else {
    `You can go check ${m} at ${u}`
}
```
<br>

### In the [Nightbot Website](https://nightbot.tv)

Add a new command then put in the name
```
!shoutout
```
Then put in the message this
```
$(eval s=`$(twitch $(touser) "{{status}}")`; g=`$(twitch $(touser) "{{game}}")`; u=`$(twitch $(touser) "{{url}}")`; t=`$(twitch $(touser) "{{uptimeLength}}")`; m=`$(touser)`; $(urlfetch PASTEBINLINK))
```
Just Change the `PASTEBINLINK` into your actual link to get the command working
