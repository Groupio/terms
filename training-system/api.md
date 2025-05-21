# ⚙️ API

Our Training system has an optional API which you can use to change the default behaviour of the product.&#x20;

![](https://cleaning.groupiotech.xyz/~gitbook/image?url=https%3A%2F%2F217617011-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FEvzv9lYLqnuj5QLpEAut%252Fuploads%252FXuH287UD4PxRcajw417s%252Fimage.png%3Falt%3Dmedia%26token%3D597f99b9-189d-42b1-88d1-8f8364c3a167\&width=768\&dpr=4\&quality=100\&sign=11c01f85\&sv=1)

## 1. API Module

The API Module is a separate module you can install for free to add alongside the Training System.&#x20;

### 1.1 Events

Events will run whenever a specific task happens with the Training System

#### 1. Loaded()

This will run when the Training System first loads.

#### 2. InformationStart(Player)

This will run when the Information starts. It gives the player who started it.

#### 3. SettingChanged(Player, Setting, NewValue)

This will run whenever a setting gets changed. It will give the player, the setting that has been changed and the new value of it.

### 1.2. Overwrites

These allow you to overwrite specific functions of the Training System

#### 1. HasPermission(Player, Task)

This will check if the given player has permission to do that set task.\
\
Return:

true - The player has permission

false - The player does not have permission

"default" - Use the default permission check.



Set this to 'nil' instead of a function to use the default permission check.



{% hint style="success" %}
Our Training System has a small API Module, however there is a large amount you can do with your own scripts already.
{% endhint %}

## 1. RemoteEvents / Functions

We use RemoteEvents or Functions within the Training System.&#x20;

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption><p>The Remotes</p></figcaption></figure>

Using these, you can create custom functionality with the training system.

For example, using :FireServer() in the remote event 'Information' will start the information if the player has permission.&#x20;

## 3. TrainingGui

We have a single module which allows changes to be made to the GUI, it also allows you to easily do certain tasks with it.

You can edit the code of this module to customize its behaviour, however this could also break the Training System.

### 3.1 :PlayTween(GuiObject, TweenInfo, PropertiesTable)

This will animate the GuiObject to have the specific properties.\
If a user has 'ReducedMotion' set as true, it will skip the animation.

### 3.2 .SendNotification(Message, From, Time, Button)

This will send a notification with the given message. It will display the picture from the UserId provided (From).

The notification will show for th egiven time, if you wish for it to be a Button set Button as true. It will return to button allowing you to create custom functionality when it is pressed.

### 3.3. ToggleHostGui(Name)

This will toggle the gui with the specific name if the player has access to it.\
It plays a small animation and ensures it is correctly displayed (E.g. viewtrainees shows all trainees)\


### 3.4. ShowMessage(Message, HostImage, TypeWriter, Camera)

This will show the given message with the picture of the host.\
It will use a typewritter effect if set as true, and play the camera animation if true.













