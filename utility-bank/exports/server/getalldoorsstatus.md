# GetAllDoorsStatus

Return the status of all the doors of a bank.

| Argument | Data Type | Nedeed                                                                       | Default | Description                         |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | ----------------------------------- |
| `bankId` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The index in the Config.Banks table |

<details>

<summary>Returns</summary>

| Type  | Description                                      |
| ----- | ------------------------------------------------ |
| table | The status of all the doors in a key value pair. |

</details>

<details>

<summary>Example</summary>

```lua
local doors = exports["utility_bank"]:GetAllDoorsStatus(1)

for door_id, status in pairs(doors) do
    print("The status of the door", door_id, "is", status)
end
```

</details>
