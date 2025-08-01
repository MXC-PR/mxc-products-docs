---
description: Find collisions in other resources
---

# FindCollisionsBetweenFiles

Find collisions between files in a resource and a list of collision files.

{% tabs %}
{% tab title="Parameters" %}
<table><thead><tr><th>Name</th><th width="86">Type</th><th width="233">Description</th><th>Default value</th></tr></thead><tbody><tr><td>resourceName</td><td>string</td><td>The name of the resource</td><td></td></tr><tr><td>files</td><td>table</td><td>The files in the resource (this will checked against collisionFiles)</td><td></td></tr><tr><td>collisionFiles</td><td>table</td><td>The files collisions (Generated with FindCollisions* functions)</td><td></td></tr></tbody></table>
{% endtab %}

{% tab title="Return" %}
<table><thead><tr><th width="290">Name</th><th width="93">Type</th><th width="312">Description</th></tr></thead><tbody><tr><td>collisions</td><td>table</td><td>A table of collisions found between files</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

