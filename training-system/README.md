---
description: >-
  In the following documentation, you can find all the important information
  about the Training System created by Groupio.
cover: .gitbook/assets/New Project (7).png
coverY: 0
---

# 🖇️ Usage of the product

<figure><img src=".gitbook/assets/New Project (4).png" alt=""><figcaption></figcaption></figure>

## 1. Training Staff Menus

There are 6 different menus that training staff can have, these are:&#x20;

### 1.1 TrainerPanel

This is the panel trainers use to interact with their assigned group.

<figure><img src=".gitbook/assets/image (5).png" alt="" width="155"><figcaption><p>The Trainer Panel</p></figcaption></figure>

**Teleport Trainees** - Teleport all the trainees **within the assigned group** to the set teleport.

**View Trainees** - View & Search all trainees in your group. Opens the ViewTrainees menu.

**Add Point Al**l - Adds a point to every trainee in the group

**Remove Point All** - Removes a point from every trainee in the group

**Pass All** - Notifies every trainee that they have passed

### 1.2. View Trainees

This allows the trainer to view all trainees within that group. They can also search for individual trainees.

<figure><img src=".gitbook/assets/image (6).png" alt="" width="153"><figcaption><p>View Trainees Panel</p></figcaption></figure>

**Username** — This allows you to type in a username. As you type, it will only show potential trainees you are searching for.

**Player Buttons** - Clicking this will open the Trainer Menu for that player.

### 1.3. Trainer Menu

<figure><img src=".gitbook/assets/image (7).png" alt="" width="528"><figcaption><p>The Trainer Menu for user 'voqalix'</p></figcaption></figure>

**Picture** - This will show a headshot of the trainee's avatar\
**Username** - This will show the trainee's username\
**Rank** - This shows the trainee's rank in the Roblox Group\
**Group** - This shows the group the trainee is assigned to

### Control Panel

**Points** - This shows the points out of the max.\
&#xNAN;_&#x54;he points bar has a  **+** and **-** sign, clicking the **+** will add a point and clicking the **-** will remove a point._

**Strikes** - This shows the amount of strikes the trainee has out of the max.\
&#xNAN;_&#x54;he strikes bar has a  **+** and **-** sign, clicking the **+** will add a strike while clicking the **-** will remove one._

**Pass Button** - This notifies the trainee that they have passed

**Fail Button** - This notifies the trainee that they have failed. If `KickIfFail` is true, they will be kicked.

### 1.4. Host Panel

This is the panel given to the host and anybody who clicks on the host part (as long as they have permission).&#x20;

&#x20;

<figure><img src=".gitbook/assets/image (10).png" alt="" width="139"><figcaption><p>The Host Panel</p></figcaption></figure>

**Sort Trainees** - This will assign all trainees in the 'Pending Team' to an active group\
**Session Options** - This allows you to change settings for the given session\
**Start Information** - This starts the Information text. If a camera animation is provided, it will play that.\
**Stage Camera** - This toggles the stage camera\
**Group Settings** - This allows you to enable/disable specific groups. \
**Teleport Trainees** - This will teleport **every** trainee to the group's teleporter

### 1.5. Session Settings (Options)

This menu allows you to change the settings for the training.&#x20;

<figure><img src=".gitbook/assets/image (11).png" alt="" width="161"><figcaption><p>The Session Settings</p></figcaption></figure>

**Session Capacity** - This controls how many trainees are sorted, trainees over the limit will be kicked.\
**PTS Requests** - This toggles if PTS requests can be made.\
**Trainee Jumping** - This toggles if players should be able to jump\
**Server Lock** - This toggles if new trainees can join.

{% hint style="info" %}
To close this frame click on the 'Session Options' button again.
{% endhint %}

### 1.6. Group Configuration (Settings)

<figure><img src=".gitbook/assets/image (14).png" alt="" width="152"><figcaption><p>The Group Configuration Menu</p></figcaption></figure>

This menu controls what groups are open (trainees can be sorted into) or closed (trainees can not be sorted into)

The text ('Group A') can be customized in the settings, however the group letters will remain the same. &#x20;

{% hint style="info" %}
To close this frame click on the 'Session Options' button again.
{% endhint %}

## 2. Training Commands

There are some commands which can be used during the training.&#x20;

1. &#x20;**!PTS**

This will send a PTS request to staff if it is enabled. Staff will be able to click the notification and teleport to the player.

**Trainer+ Commands**

2. **!Open \[DoorName]**

This will open the door with the set name

3. **!Close \[DoorName]**

This will close the door with the set name.

**Host+ Commands**

4. **!Host**

This will set yourself as the host

5. **!Cohost \[User]**

This will set the given user as the host

6. **!Trainer \[User] \[GroupLetter]**

This will set the user to be the trainer of the specific group.&#x20;

7. **!Spectator \[user]**

This will set the given user as a spectator

8. **!SetRole \[User] \[Role]**

This will set the users role to that specific role.&#x20;

9. **!Teleport \[User] \[Destination]**

Teleport the specific user to the named teleporter.

**Supervisor+ Commands**

10. **!SetHost \[User]**

This will set the given user as the host

11. **!SetTeam \[User] \[Team]**

This will put the given user on that team

12. **!SetGroup \[User] \[Group]**

This will put the given user into the given group.&#x20;
