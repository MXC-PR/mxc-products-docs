---
description: Allow to set the shutters status (closed/open)
---

# SetShuttersStatus

{% tabs %}
{% tab title="Parameters" %}
<table><thead><tr><th>Name</th><th width="112">Type</th><th width="134">Default</th><th>Description</th></tr></thead><tbody><tr><td>id</td><td>number</td><td></td><td>The store id (only 1 for now)</td></tr><tr><td>status</td><td>boolean</td><td>false</td><td>The new shutters status, true = open, false = closed</td></tr></tbody></table>
{% endtab %}

{% tab title="Returns" %}
Nothing
{% endtab %}
{% endtabs %}

## Example

<pre class="language-lua"><code class="lang-lua"><strong>exports["utility_jewelry"]:SetShuttersStatus(1, true) -- opens shutters
</strong>exports["utility_jewelry"]:SetShuttersStatus(1, false) -- closes shutters 
</code></pre>
