# GetCurrentBank

Get the id of the current bank. (Works only if the player is inside a bank)

<details>

<summary>Returns</summary>

| Type   | Description                |
| ------ | -------------------------- |
| number | The id of the current bank |

</details>

<details>

<summary>Example</summary>

```lua
local id = exports["utility_bank"]:GetCurrentBank()

print("The player is inside the bank: "..id)
```

</details>
