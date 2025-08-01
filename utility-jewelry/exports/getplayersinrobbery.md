---
description: >-
  Returns a table with all the players inside the robbery, this doesnt 100%
  means that they are robbers but only that they are near/in the robbery
  location (physically)
---

# GetPlayersInRobbery

{% tabs %}
{% tab title="Parameters" %}
<table><thead><tr><th>Name</th><th width="112">Type</th><th width="140">Default</th><th>Description</th></tr></thead><tbody><tr><td>id</td><td>number</td><td></td><td>The store id (only 1 for now)</td></tr></tbody></table>
{% endtab %}

{% tab title="Returns" %}
<table><thead><tr><th>Name</th><th width="112">Type</th><th width="140">Default</th><th>Description</th></tr></thead><tbody><tr><td>players</td><td>table</td><td></td><td>A table of all players inside the robbery (server id)</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

## Example

<pre class="language-lua"><code class="lang-lua"><strong>local players = exports["utility_jewelry"]:GetPlayersInRobbery(1)
</strong><strong>
</strong><strong>for k,v in pairs(players) do
</strong><strong>    print("The player "..GetPlayerName(v).." ("..v..") is inside the robbery")
</strong><strong>end
</strong></code></pre>
