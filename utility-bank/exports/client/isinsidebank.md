# IsInsideBank

Check if the player is inside a bank.

<details>

<summary>Returns</summary>

| Type    | Description                                          |
| ------- | ---------------------------------------------------- |
| boolean | true if the player is inside a bank, false otherwise |

</details>

<details>

<summary>Example</summary>

```lua
if exports["utility_bank"]:IsInsideBank() then
    local open = exports["utility_bank"]:IsCurrentBankDoorOpen("vault")

    print("The vault door is: "..(open and "open" or "closed"))
end
```

</details>
