---
description: Allow to get the shutters status (closed/open)
---

# GetShuttersStatus

{% tabs %}
{% tab title="Parameters" %}
<table><thead><tr><th>Name</th><th width="112">Type</th><th width="140">Default</th><th>Description</th></tr></thead><tbody><tr><td>id</td><td>number</td><td></td><td>The store id (only 1 for now)</td></tr></tbody></table>
{% endtab %}

{% tab title="Returns" %}
<table><thead><tr><th>Name</th><th width="112">Type</th><th width="140">Default</th><th>Description</th></tr></thead><tbody><tr><td>status</td><td>boolean</td><td></td><td>The store shutters status (true = open, false = closed)</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

## Example

<pre class="language-lua"><code class="lang-lua"><strong>local status = exports["utility_jewelry"]:GetShuttersStatus(1)
</strong><strong>
</strong><strong>if status then
</strong><strong>    print("Open!")
</strong><strong>else
</strong><strong>    print("Closed!")
</strong><strong>end
</strong></code></pre>
