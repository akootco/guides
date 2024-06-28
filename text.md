## Placeholders
Placeholders are ways to inject information about a player or the server into chat.
For example, I could type "Look at my cool sword $i" and `$i` would be replaced by that item's name and tooltip.
- `$i` - The item in your main hand
- `$i2` - The item in your offhand
- `$hat` - The item on your head
- `$motd` - The server's "message of the day"

These are actually placeholders for placeholders, the actual format for placeholders is:
`${player.<name>.<key>}` where `name` is their username and `key` is what you want to extract
(such as `item` or `item2`). For the server, it would be like this `${server.motd}`

There are also placeholders for player usernames:
- `@self` or `@me` - Your username
- `@random` or `@rand` - A random player's username
- `@all` or `@everyone` - Everyone's username combined in a list

## Clickable Text
Clickable text can be constructed using this format: `[Title](Content)`.
This is typically used to write URLs (all URLs will be converted to this by default),
but it can also be used to suggest or to execute commands them on click.
The command in question is always displayed when you hover over the text.
You can use color codes both in the `[Title]` section and the `(Content)` section.

### Examples
- `[&bmy website](&ahttps://akoot.co)` - **(a url)** will open a URL when clicked
- `[&n&cSend me a message](/msg Akoot_ )` - **/** will suggest that command when clicked
- `Click [&l&aHERE](!/suicide) to die instantly!` - **!/** will run that command when clicked
- `My good friend ${player.IndiaPaleAle.displayName} is in desperate need of a burrito.`

### Note...
- Don't get mad if you can't type `[`, `$`, or `}`, simply type `[[`, `$$`, or `}}` respectively.
- Some (at the time of writing, all) **clickable text** cannot be combined with **placeholders that start with $**,
i.e. `[$i2](my epic shield)` (fail!)
- Bedrock players can't interact with clickable text, 
but they will be able to see both the `Title` and `Content`.
