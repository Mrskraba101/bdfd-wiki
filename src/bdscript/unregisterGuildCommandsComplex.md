# $unregisterGuildCommands[]
Unregisters provided guild slash commands from the current guild.

## Syntax
```
$unregisterGuildCommands[Slash command name;...]
```

### Parameters
- `Slash command name` `(Type: String || Flag: Required)`: Name of the guild slash command to unregister. Use semicolons `;` as a separator to separate multiple guild slash command names.

## Example
```
$nomention

$unregisterGuildCommands[$unescape[$toLowercase[$replaceText[$trimSpace[$message]; ;]]]]
Successfully unregistered the provided guild slash commands!
```
``` discord yaml
- user_id: 1081869405245407262
  username: mrskraba101
  color: "#E67E22"
  content: |
    !example help ; anime-search ; eval
- user_id: 1009018156494368798
  username: BDFD Support
  color: "#378afa"
  bot: true
  verified: true
  content: |
    Successfully unregistered the provided guild slash commands!
```
```admonish question title="What is this?"
How [`$unescape[]`](./unescape.md), [`$toLowercase[]`](./toLowercase.md), [`$replaceText[]`](./replaceText.md), [`$trimSpace[]`](./trimSpace.md) and [`$message`](./message.md) works?
```
