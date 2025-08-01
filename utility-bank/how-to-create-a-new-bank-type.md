# How to create a new bank type

Open the config and scroll to `Config.BankTypes` \
To create a new bank type, add a table entry with your chosen name.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Every bank type require:

* [x] **coords**: Used to spawn robbery blip and calculate distance to handle _In/Out/Near_ states ([offset](how-to-create-a-new-bank-type.md#how-to-get-offset-from-interior))
* [x] **hostagesRoom**: hostages room center, used to draw intimidation bar ([offset](how-to-create-a-new-bank-type.md#how-to-get-offset-from-interior))
* [ ] **hostagesDistance**: distance from **hostagesRoom** from which onwardthe player results in the hostagesRoom (optional, default: 4.5)
* [x] **insideDistance**: distance from **coords** from which onward the player results _inside_ the bank
* [x] **nearDistance**: distance from **coords** from which onward the player results _near_ the bank
* [x] **In**: function called when the player enters the bank (please copy the In function of another&#x20;
* [x] **Out**: function called when the player exits the bank
* [x] **trollies**: table with all trollies (last coordinate is the heading) ([offset](how-to-create-a-new-bank-type.md#how-to-get-offset-from-interior))\
  &#x20;   types: cash, gold, diamond
* [x] **doors**: all doors data
* [x] **peds**: all peds data

{% hint style="info" %}
The vault hacking panel is automatically detected within a 30 meter radius of the vault door and currently only recognizes the model `hei_prop_hei_securitypanel`
{% endhint %}

After you have finished creating your bank type you can create a new bank in the `Config.Banks` that uses your newly created bank type

***

## How to get interior informations?

To retrieve interior information, use the `getInteriorInfo` command (client console).

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

## How to get offset from interior?

To determine the offset from the interior, use the `getInteriorOffset` command (client console). \
This command provides you the offset from your current position within the interior.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
