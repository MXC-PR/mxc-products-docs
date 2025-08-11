# GetRecoilStep

Return the current recoil step of the specified weapon (every time the weapon is fired, the recoil step is increased), the recoil step can be setted in Config.Patterns

| Argument | Data Type | Nedeed                                                                       | Default | Description     |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | --------------- |
| `weapon` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash |

<details>

<summary>Returns</summary>

| Type   | Description                   |
| ------ | ----------------------------- |
| number | The recoil step of the weapon |

</details>

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())

local recoilStep = exports["utility_weapons"]:GetRecoilStep(weapon)
```

</details>
