# Utility:BankRobbery:EnteredBank

Called when a player enters a bank (Called for server and the caller client)

| Argument | Data Type | Description                         |
| -------- | --------- | ----------------------------------- |
| `bankId` | number    | The index in the Config.Banks table |

<details>

<summary>Example</summary>

```lua
RegisterNetEvent("Utility:BankRobbery:EnteredBank", function(bankId)
    print("Entered bank", bankId)
end)
```

</details>
