# RemoveWeaponExperience

Remove experience from a weapon

| Argument     | Data Type | Nedeed                                                                       | Default | Description     |
| ------------ | --------- | ---------------------------------------------------------------------------- | ------- | --------------- |
| `weapon`     | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash |
| `experience` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The experience  |

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())

exports["utility_weapons"]:RemoveWeaponExperience(weapon, 100)
```

</details>
