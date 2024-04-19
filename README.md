# Twitch
stuff interacting with Twitch bots. Currently it's just lists that I pull a random entry from.

currently using a nightbot command that looks like
$(eval a=$(urlfetch json https://raw.githubusercontent.com/myUserName/myRepository/main/lists/myArray);a.filter(string => RegExp(`$(query)`,"i").test(string))[Math.floor(Math.random()*a.filter(string => RegExp(`$(query)`,"i").test(string)).length)])

that pulls a random line that matches the (case-insensitive) regex expression
