# Creating a new liquid

{% stepper %}
{% step %}
Open the `config.lua`


{% endstep %}

{% step %}
Scroll down to the section labeled `Config.Liquids`.


{% endstep %}

{% step %}
Now, you can create a new liquid.

Following this format:

```lua
["item-name"] = {
    puffs  = 10 -- The number of puffs that the liquid will last
}
```

`item-name` _refers to the name of the item that will function as a liquid._\
`puffs` _represents the number of puffs the liquid._

{% hint style="warning" %}
You need to register the item in your inventory for it to work.
{% endhint %}
{% endstep %}
{% endstepper %}
