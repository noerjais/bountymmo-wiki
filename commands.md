# Commands

You can read the list of commands that work on this server simply by writing in chat **@commands.**

The most useful are:

| Command | Example | Description |
| --- | --- | --- |
| **@autoloot number** | **@autoloot 90** | Collect into your inventory all objects from 90% to 0% rate. The max value is 100 |
| **@whodrops number**<br>**@whodrops description** | **@whodrops 4244**<br>**@whodrops Agav Card** | Describe a list of more high mobs that drop object indicated<br>(is valid ofr card, collectible or other stuff) |
| **@showexp** | | In public message chat, you can see how much exp you got (base & job) also in % |
| **@storage** | | Open your Kafra Storage everywhere you are. PS: Cannot attack with storage open |
| **@go number**<br>**@go name of town** | **@go 0**<br>**@go morroc** | Go 0 is the main city Prontera<br>Go Morror (or other name of town, teleport into main square of that town) |
| **@aloottype +N**<br>**@aloottype N** | **@aloottype +4**<br>**@aloottype -3** | Use **+** to specify an item type to always autoloot.<br>Use **-** to specify an item type to always **never** autoloot.<br>Types are: 0=healing, 2=usable, 3=etc, 4=armor, 5=weapon, 6=card, 7=pet eggs, 8=pet accessories, 10=ammo |
| **@alootid2 load N** | **@alootid2 load 1** | N can assume value from 1 to 9. Basically you can load 10 lists for your autoloot for 10 different zone. *They are commutative (do not work together). To work, you must set @autoloot to off* |
| **@alootid2 save N A B C D E F G H I L** | **@alootid2 save 1 1358 1514 1608 1152 1352 6903** | N can assume value from 1 to 9. Basically you can save 10 lists for your autoloot for 10 different zone. A B C D E F G H I L are refered to itemid (you can find the right number on RateMyServer site) |
| **@alootid2 set N** | **@alootid2 set 5** | N can assume a value from 1 to 9. Identify the list you want to autoload at the login |
| **@autoload Z** | **@autoload 1** | Z can assume value 0 or 1. Zero to turn off autoload, one to turn on autoload at login. |
| **@checkpoints** | | Show how many points you have acquired |
| **/vit+ XX** | **/vit+ 99** | Add 99 points to vit param |
| **/int+ XX** | **/int+ 99** | Add 99 points to int param |
| **/dex+ XX** | **/dex+ 99** | Add 99 points to dex param |
| **/str+ XX** | **/str+ 99** | Add 99 points to str param |
| **/agi+ XX** | **/agi+ 99** | Add 99 points to agi param |
| **/luk+ XX** | **/luk+ 99** | Add 99 points to luk param |
| **@mi X**<br>**@mi name** | **@mi 2345**<br>**@mi poring** | Information about monster indicated like drops, HP, base and job exp and other info |
| **@guildstorage** | | |
| **@time** | | Show the time server |
| **@ii object** | **@ii knife** | Information about object indicated like buy sell and weight |
