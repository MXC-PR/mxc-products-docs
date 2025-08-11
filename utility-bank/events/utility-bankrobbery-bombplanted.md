# Utility:BankRobbery:BombPlanted

Called when a bomb is planted on a prevault door,, called exactly after the item removal. (Called for server and all clients)

| Argument | Data Type | Description                                       |
| -------- | --------- | ------------------------------------------------- |
| `source` | number    | The source of the hacker                          |
| `bankId` | number    | The index in the Config.Banks table               |
| `item`   | string    | The bomb item, currently its just Config.BombItem |

<details>

<summary>Example</summary>

```lua
RegisterNetEvent("Utility:BankRobbery:BombPlanted", function(source, bankId, item)
    print("Bomb planted by", source, "in bank", bankId)
end)
```

</details>
