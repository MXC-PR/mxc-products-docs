# SetWeaponFireMode

Set the weapon fire mode of the specified weapon

| Argument | Data Type | Nedeed                                                                       | Default | Description                                                       |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | ----------------------------------------------------------------- |
| `weapon` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash                                                   |
| `mode`   | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon firemode (1 = single, 2 = burst, 3 = auto, 4 = safety) |

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())

exports["utility_weapons"]:SetWeaponFireMode(weapon, 1)
```

</details>
