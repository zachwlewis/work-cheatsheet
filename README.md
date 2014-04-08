work-cheatsheet
===============

A cheatsheet for my dang job.

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
