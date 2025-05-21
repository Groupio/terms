---
cover: .gitbook/assets/New Project (7).png
coverY: 0
---

# ⚠️ Errors

Our training system will provide errors to help you diagnose issues. This will help you work out why & potentially fix the product not working as intended.

<figure><img src=".gitbook/assets/New Project (4).png" alt=""><figcaption></figcaption></figure>

**Error messages follow the given colour scheme:**

<mark style="color:red;">**`Red`**</mark>

These errors will stop the product from working. These are more 'major' errors.

<mark style="color:orange;">**`Yellow / Orange`**</mark>

These errors usually allow the product to still work. However, it may not work as intended. These errors are 'warnings'

**`Black / Plain Text`**

This is for small messages useful for debugging.

The main usage for these messages is when something picks a suspicious activity up, and prevents the code from running due to it.

## Possible Errors

## <mark style="color:red;">1. The setting \[SettingName] has been incorrectly set up. It can not be reset to default.</mark>

You will get this error if a setting that requires an  instance (Teleports, RankDoors, CommandDoors, CameraAnimationFolder or StageCamera) has been incorrectly set up.

## <mark style="color:red;">2. Reason \[Reason] Does not exist!</mark>

You will get this error if a reason provided for HasPermission is invalid.

{% hint style="danger" %}
If you encounter this error, please report it by creating a ticket.
{% endhint %}

## <mark style="color:red;">3. Unable to find leaderstats for player</mark>

You will get this error if the training center is unable to find the leaderstats for a specific player.\
Re-joining should fix this error - Though, if encountered multiple times please report it!

## <mark style="color:red;">4. Unabile to find value 'Group' for player.</mark>

You will get this error if the training centre is unable to find the group value for a specific player.\
Re-joining should fix this error - Though, if encountered multiple times please report it!

## <mark style="color:red;">5. Unabile to find team for \[Group]</mark>

You will get this error if an active groups team can not be found.

## <mark style="color:orange;">6. The \[Type] \[Name] does not exist / can not be found and has been created.</mark>

Example:

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

You will usually get this error when something has been incorrectly set up. \
Re-add the product, and use the plugin to set it up.

{% hint style="success" %}
The Training system should attempt to resolve this error by creating the instances when it has loaded. However, to speed up loading times and to silence the error it is better to have them existing already.
{% endhint %}



## <mark style="color:orange;">7. The owner of this experience does not have the licence for the Training System by Groupio. Version: \[VersioNumber]</mark>

You will get this error if the owner does not have the correct licence for the Training System. If you wish to give the owner the licence, you can gift the user in hour Hub or request a transfer.

## <mark style="color:orange;">8. No trainings module has been found - Settings have been reset to default</mark>

You will get this error if there is no ModuleScript for the training settings.\
It will reset all settings to the default values.

## <mark style="color:orange;">9. The Setting \[SettingName] has been incorrectly set up and has been reset to default \[DefaultValue]</mark>

You will get this error when a setting is incorrectly set up (The wrong type)

## <mark style="color:orange;">10. The setting \[Setting] is now deprecated . Please use \[NewSetting] instead.</mark>

You will get this error for using a deprecated setting. We highly recommend you switch to using the new  setting instead.

## <mark style="color:orange;">11. Attempt to set \[Setting] as a boolean</mark>&#x20;

You will get this error if a piece of code attempts to set a Training Setting that is not a boolean (true/false) as one.

## <mark style="color:orange;">12. Group \[NewValue] does not exist!</mark>

You will get this error if a piece of code attempts to toggle a group that does not exist.

## <mark style="color:orange;">13. Setting \[SettingName] can not be changed!</mark>

You will get this error if you attempt to change a setting which can not be changed.
