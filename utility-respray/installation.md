# Installation

{% stepper %}
{% step %}
### 📦Required Dependencies

* [ ] Install [Utility Lib](https://github.com/utility-library/utility_lib)
{% endstep %}

{% step %}
### :ox: Add the spraygun to the ignored weapon list (ox\_inventory)

Add the following [convar](https://docs.fivem.net/docs/scripting-reference/convars/) to your `server.cfg` to prevent `ox_inventory` from removing the spraygun weapon

```
setr inventory:ignoreweapons ["WEAPON_SPRAYGUN"]
```

Save the changes and restart your server to apply the configuration

{% hint style="warning" %}
If you already have the `inventory:ignoreweapons` [convar](https://docs.fivem.net/docs/scripting-reference/convars/) set elsewhere in your `server.cfg`, simply add `WEAPON_SPRAYGUN` to the existing array.\
For example, if your current array is `["WEAPON_KNIFE", "WEAPON_BAT"]`, update it to `["WEAPON_KNIFE", "WEAPON_BAT", "WEAPON_SPRAYGUN"]`.&#x20;

Make sure each weapon is separated by a comma and enclosed in double quotes.
{% endhint %}
{% endstep %}
{% endstepper %}

