---
cover: .gitbook/assets/New Project (7).png
coverY: 0
---

# 🖌️ Customization of the product

Our Training System provides you with the ability to customize the system to make it more useful for you & your training center!

<figure><img src=".gitbook/assets/New Project (4).png" alt=""><figcaption></figcaption></figure>

**Workspace:**\
These can be customized in Workspace. It is recommended to do this when setting up our Training System.

## 1. Doors

In 'Workspace' you will see a folder named 'Doors'. These will automatically become invisible when the game starts, and you can only see them in studio.

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption><p>Default Doors folder in Workspace</p></figcaption></figure>

These are the doors the training system interacts with, they have two categories:

### 1.1 CommandDoors

These doors are seen as a green forcefield in Roblox Studio and can be toggled by the !open and !close commands.&#x20;

For example, !open DoorA will allow anybody to walk through DoorA.&#x20;

#### Creating new command doors

To create a new command door, you can duplicate the current door ('DoorA') or create a new part and place it in that folder.\
Doors can be resized, moved or rotated. You can also change the properties.

{% hint style="danger" %}
All Command Doors **must** have a unique name. This is the name used by the command. Try keep these names simple for trainers to use and remember.
{% endhint %}

### 1.2 RankDoors

These are doors seen as a red forcefield in Roblox Studio by default. \
People above the Trainer Rank will be able to walk through these doors, anybody else will not.

#### Creating new Rank Doors

To create a new rank door, you can duplicate the current door ('RankA') or create a new part and place it in that folder.&#x20;

Doors can be resized, moved or rotated. You can also change the properties.

{% hint style="danger" %}
Please make sure 'Anchored' is set as true for both Command & RankDoors.&#x20;

If 'Anchored' is false, the door will fall through the map and can not be closed.
{% endhint %}

## 2. Teleports

These are the locations a player is able to teleport to through the !teleport command or teleport trainees button.\
They are shown as 1x1x1 yellow forcefield cubes in Roblox Studio. Like Doors, they are made invisible when the game starts.

<figure><img src=".gitbook/assets/image (25).png" alt=""><figcaption><p>Picture of the default Teleports in Workspace</p></figcaption></figure>

There is two types of teleport location:

### 2.2 Group Teleports

These are the locations that the trainees teleport to when 'Teleport Trainees' is pressed. \
It must be named the letter of the group. For example, The destination where trainees in group B will teleport to should be named 'B'

All 4 of these teleporters come with the training system by default, you just need to move this to where you want them to teleport to.

### 2.2. Custom Teleports

These are teleport locations only available by using the !teleport command.\
For example, !teleport Jay CustomTeleportLocation will teleport Jay to the position of the CustomTeleportLocation part

#### Creating new Teleports

You can duplicate any teleport location and rename it. You could also create a new part and insert it under the teleports folder. It is recommended to have the size as 1x1x1 so you can accurately locate where the player will teleport to. (The center of the part)

{% hint style="danger" %}
Anchored must be set as true, if it is false the teleport locations may fall through the map and get destroyed.
{% endhint %}

## 3. Cameras

There is two cameras you can customize within the Training System. \
The parts will be hidden in game. &#x20;

A CameraPart in Roblox Studio will look like this:

The two surfaces show you the direction the camera will be looking at.&#x20;

<figure><img src=".gitbook/assets/image (30).png" alt="A picture of the Camera Part for the Stage Camera" width="523"><figcaption><p>A picture of a CameraPart</p></figcaption></figure>

Stud: This is seen at the top of the part. \
This shows you where the top of the camera will be.

{% hint style="success" %}
To avoid the camera being sideways or upsidedown. It is recommended to keep this pointing up. (Can be tilted to tilt the camera, as showin in the picture)
{% endhint %}

The hinge is pointing in the direction the camera will be looking at.&#x20;

The CameraPart above will show this:

<figure><img src=".gitbook/assets/image (27).png" alt="" width="563"><figcaption><p>A picture of what the Camera will show</p></figcaption></figure>

### 3.1 StageCamera

This is the camera that will be shown to trainees when 'Stage Camera' is toggled.

This is a single part under Workspace

<figure><img src=".gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

You can move or rotate this to change the stage camera

### 3.2. Information Camera

This is the camera animation that plays while the information is active

<figure><img src=".gitbook/assets/image (32).png" alt=""><figcaption><p>The Camera Animation Structure</p></figcaption></figure>

It has seperate folders, each with multiple camera parts.&#x20;

The code will go through each folder individually, and then tween between the cameras in the number order given  (1,2,3,4,5)\
It will teleport to Camera 1, but then move to 2, 3, 4...

{% hint style="info" %}
After finished customizing the cameras, you can move them to ReplicatedStorage so they are out of your way when developing. Make sure to update your settings though!
{% endhint %}



## 4. Settings

The training system has settings which can be changed to customize the Training System

### 4.1. GroupId

This is the Id of your Roblox Group. This setting is required

### 4.2. Trainer Rank

This is the minimum rank id which has Trainer permissions. This setting is required.

### 4.3. Host Rank

This is the minimum rank id which has Host permissions. This setting is required.

### 4.4. Supervisor Permission

This is the minimum rank id which has supervisor permisson. This setting is required.

### 4.5. Name

This is the Name of the training center, used with {name} for information messages. It is required if you use it.&#x20;

### 4.6. DoorsFolder

This is the folder for the [doors](customization-of-the-product.md#id-1.-doors). This is not a setting, and if the CommandDoors and RankDoors are parented to Workspace you do not need it.

### 4.7. Disabled Commands

These are default training system commands which can not be used by anybody.

To  add a command, add it into the list. For example&#x20;

```lua
DisabledCommands = {"pts", "teleport"}
```

Will disable the pts and teleport commands.&#x20;

### 4.8. ExtraRoles

These are extra roles you can add to use alongside the !role command.

{% hint style="info" %}
Trainee, Host, Cohost & Spectator are all roles by default. You do not need to add these.\
\
Only "trainee" works with the !role command, others have their own individual commands.
{% endhint %}

### 4.9 Training Teams

These are teams used by the training staff

```lua
TrainingTeams = {
		HostTeam = "TEAMNAME";
		TrainingStaffTeam = "TEAMNAME";
		TraineeTeam = "TEAMNAME";
		SpectatorTeam = "TEAMNAME";
		PendingTeam = "TEAMNAME";
	};
```

Set 'TEAMNAME' to the name you wish the team to have.&#x20;

{% hint style="info" %}
To 'remove' or merge two (or more) teams, you can set them both to have the same name.
{% endhint %}

### 4.10 GroupsUseTeams

This will toggle if the groups will show up in teams.

true = They will show up

false = they won't

### 4.11. TrainingGroups

```lua
TrainingGroups = {
		["A"] = "Group A";
		["B"] = "Name Here";
		["C"] = "";
		["D"] = "Unknown Group";

	};
```

The letters must remain the same, however setting the name of the group will change it in both teams & on the host menu.

{% hint style="info" %}
As shown for Group C, having a group name empty will disable the group - Meaning the host can not use that one. It will also not create a team.
{% endhint %}

### 4.12. ShowGroupOnLeaderstats

This will toggle if groups should show as a leaderstats value.\
Groups will show the letter (A,B,C or D)

true = it will show

false = it will not show.

### 4.13. ServerLockMessage

This is the message that will be shown when a player is kicked due to the server being locked.

### 4.14. MaxPoints

This is the maximum amount of points a player can recieve

### 4.15. MaxStrikes

This is the maximum amount of strikes a player can recieve

### 4.16. ShowPoints

This toggles if points should be shown as a leaderstats value

### 4.17. ShowStrikes

This toggles if strikes should be shown as a leaderstats value

### 4.18. Autofail

This will toggle if the user should be failed when recieving the maximum amount of points.

### 4.19. KickifFailed

This will toggle if a player is kicked for failing the training

### 4.20. BypassServerLockRank

This is the minimal rank id which can join even if the server is locked

### 4.21. OnlyAllowGroup

This toggles if only group members are allowed to join, non group members will be kicked.

### 4.22. PTS

This toggles if the PTS system is used, if not it is disabled and the host can not toggle it.

### 4.23. AntiCheatKicks

This toggles if the anti cheat will kick players

{% hint style="danger" %}
Due to the possibility of false detections, it is recommended to leave this as false.&#x20;
{% endhint %}

### 4.24. CommandPrefix

This is the prefix used for the training systems commands. It should only be 1 character.

### 4.25. Messages

This is a list of messages shown when 'Show Information' is pressed.

Using {name} will use the training centers name provided in the settings, and {host} will provide the hosts name.

### 4.26. TypewriterEffect

This toggles if a type writer effect is visible for Information.

### 4.27. CharacterWait

This is the time between showing a character when the Typewriter effect is set as true.

### 4.28. Teleports

This is the folder containing all teleport locations for the Training System

### 4.29. RankDoors

This is the folder containing all the rank doors for the Training System

### 4.30. CommandDoors

This is the folder containing all of the command doors for the training system.

### 4.31. InformationCamera

If the camera should change (and move) during information.

### 4.32. CameraAnimationFolder

This is the folder for the[ information camera](customization-of-the-product.md#id-3.2.-information-camera) animations.

### 4.33. CameraTime

This is the minimal amount of time the information will be active for. This is used for if you want the camera to show after the information text.&#x20;

<details>

<summary>Working out Information Time</summary>

If the Camera Time is less than the Text time, it will not be used.\
Text Ti[me ≈ (CharacterWait \* TotalNumberOfCharacters) + 3.5](#user-content-fn-1)[^1]\
\
If TextTime > CameraTime then\
InformationTime = TextTime

\
However, if the CameraTime is bigger than the TextTime then\
InformationTime = TextTime + (CameraTime - TextTime)

</details>

### 4.34. StageCamera

This is the part used to view the stage camera

### 4.35. Debug

This toggles if Debug information should be outputted to the console to help identify errors.

## 5. TrainingConfig

There is a Configuration that comes with our Training System to alter the default settings used when the training starts. This is found in ReplicatedStorage

<figure><img src=".gitbook/assets/image (33).png" alt=""><figcaption><p>TrainingConfig in ReplicatedStorage</p></figcaption></figure>

The settings can be found as attributes at the bottom of the Properties.

<figure><img src=".gitbook/assets/image (34).png" alt=""><figcaption><p>TrainingConfig Settings</p></figcaption></figure>

These are used by the code, and also automatically updated whenever a setting is changed.&#x20;

{% hint style="warning" %}
These settings are defaults, the Host will be able to change these.&#x20;
{% endhint %}

[^1]: TextTime may vary, However this is a very small difference and does not need to be considered.
