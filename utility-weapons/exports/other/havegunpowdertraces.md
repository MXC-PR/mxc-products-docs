# HaveGunpowderTraces

Return true if the player has a gunpowder trace.

| Argument | Data Type | Nedeed                                                               | Default | Description             |
| -------- | --------- | -------------------------------------------------------------------- | ------- | ----------------------- |
| `source` | number    | <ul class="contains-task-list"><li><input type="checkbox"></li></ul> | `-`     | Only in the server side |

<details>

<summary>Returns</summary>

| Type    | Description                            |
| ------- | -------------------------------------- |
| boolean | If the player is holding breath or not |

</details>

<details>

<summary>Example</summary>

The following example shows how to use the export in the client-side, for the server side you need to use the `source` argument.

```lua
exports["utility_weapons"]:HaveGunpowderTraces()
```

</details>
