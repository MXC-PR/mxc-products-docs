# GetWeaponExperience

Return the experience of the specified weapon

| Argument | Data Type | Nedeed                                                                       | Default | Description     |
| -------- | --------- | ---------------------------------------------------------------------------- | ------- | --------------- |
| `weapon` | number    | <ul class="contains-task-list"><li><input type="checkbox" checked></li></ul> | `-`     | The weapon hash |

<details>

<summary>Returns</summary>

| Type   | Description                                        |
| ------ | -------------------------------------------------- |
| number | The experience that the player has with the weapon |

</details>

<details>

<summary>Example</summary>

```lua
local retval, weapon = GetCurrentPedWeapon(PlayerPedId())
local experience = exports["utility_weapons"]:GetWeaponExperience(weapon)

print(experience)
```

</details>
