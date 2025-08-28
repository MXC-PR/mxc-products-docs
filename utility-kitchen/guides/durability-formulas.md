# Durability formulas

This documentation explains how durability is calculated for ingredients/food&#x73;**.**

***

## Ingredient/Food Durability

Each ingredient (or food item that can be cooked) has a **durability value** depending on how well it is cooked.

The <mark style="color:$success;">**perfect cooking point**</mark> is at <mark style="color:$success;">**73% (0.73)**</mark> of its cooking progress.

Durability scales as follows:

1. **From 0** → **0.73 cooking progress**
   * Durability rises from **0%** → **100%**
   * Example: <mark style="color:yellow;">halfway cooked</mark> (0.365) gives \~50% durability.
2. **From 0.73 → 1.00 cooking progress**
   * Durability decreases from **100% → 0%**
   * Example: <mark style="color:red;">burned</mark> (1.0) gives 0% durability.

The progressbar is completed at <mark style="color:$success;">73%</mark> after that it will start turning <mark style="color:red;">red</mark> and so <mark style="color:red;">burning</mark>

***

### Examples

Cooking progress = <mark style="color:orange;">**0.50**</mark>\
Durability = <mark style="color:$info;">(0.50 / 0.73) \* 100</mark> \
&#x20;                  ≈ <mark style="color:orange;">69%</mark>

<div align="left"><figure><img src="../../.gitbook/assets/70.webp" alt="" width="64"><figcaption></figcaption></figure></div>

Cooking progress = <mark style="color:red;">**0.90**</mark>\
Durability = <mark style="color:$info;">((1 - 0.90) / (0.27)) \* 100</mark>\
&#x20;                  \= <mark style="color:$info;">(0.10 / 0.27) \* 100</mark>\
&#x20;                  ≈ <mark style="color:red;">37%</mark>

<div align="left"><figure><img src="../../.gitbook/assets/126.webp" alt="" width="64"><figcaption></figcaption></figure></div>

Cooking progress = <mark style="color:$success;">**0.73**</mark>\
Durability = <mark style="color:$info;">(0.73 / 0.73) \* 100</mark>\
&#x20;                  \= <mark style="color:$info;">1 \* 100</mark>\
&#x20;                  \= <mark style="color:$success;">100%</mark>

<div align="left"><figure><img src="../../.gitbook/assets/100.webp" alt="" width="64"><figcaption></figcaption></figure></div>

***

## Hamburger Durability

A hamburger’s durability depends on **two factors**:

1. <mark style="color:blue;">How well its ingredients are cooked.</mark>
2. <mark style="color:orange;">How many ingredients are used.</mark>

***

### 1. <mark style="color:blue;">Ingredient Durability (80% of total)</mark>

Each ingredient contributes durability based on how close it is to the **perfect cooking point** (73%).\
We take the **average durability** of all ingredients in the burger.

👉 Example:

* 4 ingredients with durabilities **60%, 80%, 90%, 70%**
* Average durability = (60 + 80 + 90 + 70) / 4 = **75%**

### 2. <mark style="color:orange;">Ingredient Count Score (20% of total)</mark>

The hamburger also gets a bonus depending on how many ingredients it has.\
Max bonus at <mark style="color:$success;">**8 ingredients = 100%**</mark><mark style="color:$success;">.</mark>\
Fewer ingredients give a smaller bonus.

| Ingredients | Score |
| ----------- | ----- |
| 8           | 100%  |
| 6           | 75%   |
| 4           | 50%   |
| 2           | 25%   |
| 0           | 0%    |

👉 Example:

* 4 ingredients = <mark style="color:orange;">**50% score**</mark>

***

### Combine Them (Final Durability)

The final durability of the hamburger is calculated as:

<mark style="color:green;">Hamburger Durability</mark> = (<mark style="color:blue;">Average Ingredients Durability</mark> \* 0.8) + (<mark style="color:orange;">Ingredient Count Score</mark> \* 0.2)

#### Example:

Average ingredients durability = <mark style="color:blue;">**75% (0.75)**</mark>\
Ingredient count score = <mark style="color:orange;">**50% (0.50)**</mark>

Durability = (<mark style="color:blue;">0.75</mark>\*0.8) + (<mark style="color:orange;">0.50</mark>\*0.2) \* 100\
&#x20;                  \= <mark style="color:blue;">0.60</mark> + <mark style="color:orange;">0.10</mark> \* 100\
&#x20;                  \= <mark style="color:green;">70%</mark>

***

### Examples

**2 ingredients (cooked at 0.5, 0.6) and 6 filling ingredients**

Ingredient durabilities:\
0.5 → 68%\
0.6 → 82%\
Average = <mark style="color:blue;">**75%**</mark>

Ingredient count score: \
<mark style="color:$info;">(8 / 8) \* 100</mark> = <mark style="color:orange;">100%</mark>

Final durability:\
(<mark style="color:blue;">75</mark> \* 0.8) + (<mark style="color:orange;">100</mark> \* 0.2) = <mark style="color:blue;">60</mark> + <mark style="color:orange;">20</mark> = <mark style="color:green;">62%</mark>

***

#### 5 filling ingredients, no cooking ingredient

Ingredient durabilities:\
(none, so all = <mark style="color:blue;">0%</mark>)\
Average = <mark style="color:blue;">0%</mark>

Ingredient count score:\
<mark style="color:$info;">(5 / 8) \* 100</mark> = <mark style="color:orange;">62%</mark>

Final durability:\
(<mark style="color:blue;">0</mark> \* 0.8) + (<mark style="color:orange;">62</mark> \* 0.2) = <mark style="color:blue;">0</mark> + <mark style="color:orange;">12</mark> = <mark style="color:green;">12%</mark>

***

#### 1 cooking ingredient burned (1.0) and 2 filling ingredients

Ingredient durabilities:\
1.0 → 0%\
Average = <mark style="color:blue;">0%</mark>

Ingredient count score:\
<mark style="color:$info;">(3 / 8) \* 100</mark> = <mark style="color:orange;">37%</mark>

Final durability:\
(<mark style="color:blue;">0</mark> \* 0.8) + (<mark style="color:orange;">37</mark> \* 0.2) = <mark style="color:blue;">0</mark> + <mark style="color:orange;">7</mark> = <mark style="color:green;">7%</mark>
