# SetBankDoorStatus

Sets the status of a bank door.

| Argument | Data Type | Nedeed                                                                       | Default | Description                                                                                            |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------ |
| `bankId` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The index in the Config.Banks table                                                                    |
| `doorId` | string    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | Internal id to refer the door, generally can be one of the following values: vault, prevault, shutters |
| `status` | boolean   | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | True to open the door, false to close it (for shutters its inverted, so true = closed)                 |

<details>

<summary>Example</summary>

```lua
exports["utility_bank"]:SetBankDoorStatus(1, "shutters", true)
```

</details>
