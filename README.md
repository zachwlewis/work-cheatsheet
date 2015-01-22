work-cheatsheet
===============

A cheatsheet for my dang job.

Contents
--------
1. [Integrating Changelists](https://github.com/zachwlewis/work-cheatsheet#integrating-changelists)
2. [Useful Command Line Arguments](https://github.com/zachwlewis/work-cheatsheet#useful-command-line-arguments)
3. [Launch URLs](https://github.com/zachwlewis/work-cheatsheet#launch-urls)
4. [Native Script Classes](https://github.com/zachwlewis/work-cheatsheet#native-script-classes)

Integrating Changelists
-----------------------

1. Submit to development branch.
2. Switch to release branch.
3. Right-click submitted changelist and select <kbd>Merge/Integrate...</kbd>.
4. Select the appropriate branch mapping.
5. Accept the merge.
6. Interactively resolve each file in the pending changelist.
7. Test the release build.
8. Submit the pending changelist with the following description:

```
Source_Branch_Name -> Target_Branch_Name [CL <source changelist number>]
<source changelist description>
```

Useful Command Line Arguments
----------------------------

|Command|Description|
|-----------|-----------|
|`-windowed`|Launches the game windowed|
|`-log`|Shows the log window.|

Launch URLs
-----------

|URL Command|Description|
|-----------|-----------|
|`DisplayNameDialog`|Displays the name dialog for supported gametypes.|
|`HideMenuOnMapLoad`||
|`RoleName=<role>`|Sets the client's role.|

Native Script Classes
---------------------

When declaring a script class as native, it must be implemented in native code. For Actors, start the class with `A`. For Objects, start the class with `U`.

``` java
/** MyNativePawn.uc */
class MyNativePawn extends Pawn
  native;
```

``` cpp
IMPLEMENT_CLASS(AMyNativePawn);

void AMyNativePawn::foo()
{
  // Native function body.
}
```
