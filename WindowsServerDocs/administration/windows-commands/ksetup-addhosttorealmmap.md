---
title: ksetup:addhosttorealmmap
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 237742d5-fa68-466c-b97e-636f489248ea
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# ksetup:addhosttorealmmap



Adds a service principal name (SPN) mapping between the stated host and the realm.

## Syntax

```
ksetup /addhosttorealmmap <HostName> <RealmName>
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|\<HostName>|The host name is the computer name, and it can be stated as the computer's fully qualified domain name.|
|\<RealmName>|The realm name is stated as an uppercase DNS name, such as CORP.CONTOSO.COM.|

## Remarks

This command allows you to map a host or multiple hosts that are sharing the same DNS suffix to the realm.

The mapping is recorded in the registry in **HKEY_LOCAL_MACHINE\SYSTEM\CurrentContolSet\Lsa\Kerberos\HostToRealm**.

## Examples

As part of configuring the realm CONTOSO, map the host computer IPops897 to the realm:
```
ksetup /addhosttorealmmap IPops897 CONTOSO
```
Verify in the registry that the mapping is as intended.

## Additional References

-   [Ksetup:delhosttorealmmap](ksetup-delhosttorealmmap.md)
-   [Ksetup](ksetup.md)
-   - [Command-Line Syntax Key](command-line-syntax-key.md)