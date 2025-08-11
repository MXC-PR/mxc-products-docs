# IsWeaponJammed

Return the jammed state of the specified weapon

| Argument | Data Type | Nedeed                                                                       | Default | Description     |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | --------------- |
| `weapon` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash |

<details>

<summary>Returns</summary>

| Type    | Description                    |
| ------- | ------------------------------ |
| boolean | The jammed state of the weapon |

</details>

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())

local jammed = exports["utility_weapons"]:IsWeaponJammed(weapon)
```

</details>
