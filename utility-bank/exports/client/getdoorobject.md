# GetDoorObject

Get the object (entity) of a door or 0 if not found.

| Argument | Data Type | Nedeed                                                                       | Default | Description                                                                                            |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------ |
| `bankId` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The index in the Config.Banks table                                                                    |
| `doorId` | string    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | Internal id to refer the door, generally can be one of the following values: vault, prevault, shutters |

<details>

<summary>Returns</summary>

| Type   | Description                     |
| ------ | ------------------------------- |
| number | The object (entity) of the door |

</details>

<details>

<summary>Example</summary>

```lua
local obj = exports["utility_bank"]:GetDoorObject(1, "shutters")

print(GetEntityCoords(obj))
```

</details>
