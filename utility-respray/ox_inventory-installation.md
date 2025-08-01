# 🐂 ox\_inventory (Installation)

This guide explains how to properly install and configure `utility_respray` for use with `ox_inventory`.\
To ensure compatibility, you need to add the **spraygun** to the `inventory:ignoreweapons` [convar](https://docs.fivem.net/docs/scripting-reference/convars/) in your server configuration.

## Installation Steps

* [ ] Add the following convar to your `server.cfg` to prevent `ox_inventory` from removing the spraygun weapon

{% code fullWidth="false" %}
```
setr inventory:ignoreweapons ["WEAPON_SPRAYGUN"]
```
{% endcode %}

* [ ] Save the changes to your `server.cfg`.
* [ ] Restart your server to apply the configuration

{% hint style="warning" %}
If you already have the `inventory:ignoreweapons` convar set elsewhere in your `server.cfg`, simply add `WEAPON_SPRAYGUN` to the existing array.\
For example, if your current array is `["WEAPON_KNIFE", "WEAPON_BAT"]`, update it to `["WEAPON_KNIFE", "WEAPON_BAT", "WEAPON_SPRAYGUN"]`.&#x20;

Make sure each weapon is separated by a comma and enclosed in double quotes.
{% endhint %}
