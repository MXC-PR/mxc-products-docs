# IsCurrentBankDoorOpen

Check if the current bank door is open. (Works only if the player is inside a bank)

| Argument | Data Type | Nedeed                                                                       | Default | Description                                                                                            |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------ |
| `doorId` | string    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | Internal id to refer the door, generally can be one of the following values: vault, prevault, shutters |

<details>

<summary>Returns</summary>

| Type    | Description                               |
| ------- | ----------------------------------------- |
| boolean | true if the door is open, false otherwise |

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
