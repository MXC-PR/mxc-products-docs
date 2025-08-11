# Utility:BankRobbery:VaultHacked

Called when a bank vault is hacked. (Called for server and all clients)

| Argument | Data Type | Description                         |
| -------- | --------- | ----------------------------------- |
| `source` | number    | The source of the hacker            |
| `bankId` | number    | The index in the Config.Banks table |

<details>

<summary>Example</summary>

```lua
RegisterNetEvent("Utility:BankRobbery:VaultHacked", function(source, bankId)
    print("Vault hacked by", source, "in bank", bankId)
end)
```

</details>
