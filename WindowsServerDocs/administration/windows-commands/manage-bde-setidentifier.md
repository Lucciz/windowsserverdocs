---
title: manage-bde setidentifier
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 7092d18f-4ac9-4c73-a20f-1246ca60e75e
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# manage-bde: setidentifier



Sets the drive identifier field on the drive to the value specified in the **Provide the unique identifiers for your organization** Group Policy setting.

## Syntax

```
manage-bde –setidentifier <Drive> [-computername <Name>] [{-?|/?}] [{-help|-h}]
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|\<Drive>|Represents a drive letter followed by a colon.|
|-computername|Specifies that Manage-bde.exe will be used to modify BitLocker protection on a different computer. You can also use **-cn** as an abbreviated version of this command.|
|\<Name>|Represents the name of the computer on which to modify BitLocker protection. Accepted values include the computer's NetBIOS name and the computer's IP address.|
|-? or /?|Displays brief Help at the command prompt.|
|-help or -h|Displays complete Help at the command prompt.|

## Examples

To illustrates using the **-setidentifier** command to set BitLocker drive identifier field for C.
```
manage-bde –setidentifier C:
```

## Additional References

-   - [Command-Line Syntax Key](command-line-syntax-key.md)
-   [Manage-bde](manage-bde.md)
-   [Using Data Recovery Agents with BitLocker](https://technet.microsoft.com/library/dd875560(WS.10).aspx)