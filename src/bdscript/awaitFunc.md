# $awaitFunc
Used to initiate an awaited command.

## Syntax
```
$awaitFunc[name;(user ID;channel ID)]
```

### Parameters
- `name` `(Type: String || Flag: Required)`: The name used inside [`$awaitedCommand[]`](../callbacks/awaitedCommand.md) and [`$awaitedCommandError[]`](../callbacks/awaitedCommandError.md) callbacks.
- `user ID` `(Type: Snowflake || Flag: Vacantable)`: The user the awaited command will trigger for. Uses command author, if `user ID` is not given.
- `channel ID` `(Type: Snowflake || Flag: Optional)`: The channel where the command will be awaited. Uses current channel, if `channel ID` is not given.

## Example
```
$nomention
What do you want me to say?
$awaitFunc[say]
```

