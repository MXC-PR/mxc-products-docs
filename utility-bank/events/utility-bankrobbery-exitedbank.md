# Utility:BankRobbery:ExitedBank

Called when a player exits a bank (Called for server and the caller client)

| Argument | Data Type | Description                         |
| -------- | --------- | ----------------------------------- |
| `bankId` | number    | The index in the Config.Banks table |

<details>

<summary>Example</summary>

```lua
RegisterNetEvent("Utility:BankRobbery:ExitedBank", function(bankId)
    print("Exited bank", bankId)
end)
```

</details>
