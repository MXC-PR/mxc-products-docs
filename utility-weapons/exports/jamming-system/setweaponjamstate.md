# SetWeaponJamState

Set the weapon jam state of the specified weapon

| Argument | Data Type | Nedeed                                                                       | Default | Description     |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | --------------- |
| `weapon` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash |
| `state`  | boolean   | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The jam state   |

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())

exports["utility_weapons"]:SetWeaponJamState(weapon, true)
```

</details>
