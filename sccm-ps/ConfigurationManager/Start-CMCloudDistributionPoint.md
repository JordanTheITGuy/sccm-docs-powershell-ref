<<<<<<< HEAD
---
title: Start-CMCloudDistributionPoint
titleSuffix: Configuration Manager
description: Starts the cloud distribution point service.
ms.date: 05/07/2019
ms.prod: configuration-manager
ms.technology: configmgr-other
ms.topic: conceptual
author: aczechowski
ms.author: aaroncz
manager: dougeby
=======
﻿---
external help file: AdminUI.PS.Content.dll-Help.xml
ms.assetid: 0F8788AA-2C2A-4834-9CEA-9390D1E67F52
online version: https://go.microsoft.com/fwlink/?linkid=834207
schema: 2.0.0
>>>>>>> master
---

# Start-CMCloudDistributionPoint

## SYNOPSIS
Starts the cloud distribution point service.

## SYNTAX

### SearchByValueMandatory (Default)
```
Start-CMCloudDistributionPoint -InputObject <IResultObject> [-DisableWildcardHandling] [-ForceWildcardHandling]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SearchByIdMandatory
```
Start-CMCloudDistributionPoint -Id <String> [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### SearchByNameMandatory
```
Start-CMCloudDistributionPoint -Name <String> [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Start-CMCloudDistributionPoint** cmdlet starts the cloud distribution point service.

You can use the [Stop-CMCloudDistributionPoint](Stop-CMCloudDistributionPoint.md) cmdlet to suspend distribution of content.

## EXAMPLES

> [!NOTE]
> Configuration Manager CmdLets must be run from the Configuration Manager site drive. For more information, see the [getting started documentation](https://docs.microsoft.com/powershell/sccm/overview).


### Example 1: Start the cloud distribution point service using an ID
```
PS XYZ:\> Start-CMCloudDistributionPoint -Id "16777242"
```

This command starts the cloud distribution point service for the cloud distribution point that has the specified identifier.

### Example 2: Start the cloud distribution point service using a name
```
PS XYZ:\> Start-CMCloudDistributionPoint -Name "West01"
```

This command starts the cloud distribution point service for the cloud distribution point named West01.

### Example 3: Start the cloud distribution point service using an object
```
PS XYZ:\> $DistPnt = Get-CMCloudDistributionPoint -Id "16777242"
PS XYZ:\> Start-CMCloudDistributionPoint -InputObject $DistPnt
```

The first command uses the **Get-CMCloudDistributionPoint** cmdlet to get the distribution point with the specified identifier, and then saves it in the $DistPnt variable.

The second command starts the cloud distribution point service for the distribution point stored in $DistPnt.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableWildcardHandling
DisableWildcardHandling treats wildcard characters as literal character values. Cannot be combined with **ForceWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
ForceWildcardHandling processes wildcard characters and may lead to unexpected behavior (not recommended). Cannot be combined with **DisableWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Specifies an array of identifiers for cloud distribution points.
You can use a comma-separated list.

```yaml
Type: String
Parameter Sets: SearchByIdMandatory
Aliases: AzureServiceId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Specifies a cloud distribution point object.
To obtain a cloud distribution point object, you can use the [Get-CMCloudDistributionPoint](Get-CMCloudDistributionPoint.md) cmdlet.

```yaml
Type: IResultObject
Parameter Sets: SearchByValueMandatory
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of a cloud distribution point.

```yaml
Type: String
Parameter Sets: SearchByNameMandatory
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-CMCloudDistributionPoint](Get-CMCloudDistributionPoint.md)

[New-CMCloudDistributionPoint](New-CMCloudDistributionPoint.md)

[Remove-CMCloudDistributionPoint](Remove-CMCloudDistributionPoint.md)

[Set-CMCloudDistributionPoint](Set-CMCloudDistributionPoint.md)

[Stop-CMCloudDistributionPoint](Stop-CMCloudDistributionPoint.md)
