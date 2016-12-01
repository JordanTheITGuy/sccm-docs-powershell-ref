---
external help file: AdminUI.PS.Hybrid.dll-Help.xml
online version: https://go.microsoft.com/fwlink/?linkid=833728
schema: 2.0.0
ms.assetid: C45DD606-A366-49CA-AA64-AAD1285340D9
---

# Get-CMIntuneSubscription

## SYNOPSIS
Gets a Microsoft Intune subscription.

## SYNTAX

```
Get-CMIntuneSubscription [-DisableWildcardHandling] [-ForceWildcardHandling] [<CommonParameters>]
```

## DESCRIPTION
The **Get-CMIntuneSubscription** cmdlet gets the properties of a Microsoft Intune subscription in Microsoft System Center Configuration Manager.

## EXAMPLES

### Example 1: Get the Microsoft Intune subscription
```
PS C:\> Get-CMIntuneSubscription
```

This command gets the Microsoft Intune subscription for the Configuration Manager site.

## PARAMETERS

### -DisableWildcardHandling
Indicates that wildcard handling is disabled.

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
Indicates that wildcard handling is enabled.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### IResultObject#SMS_CloudSubscription

## NOTES

## RELATED LINKS

[Add-CMIntuneSubscription](./Add-CMIntuneSubscription.md)

[Remove-CMIntuneSubscription](./Remove-CMIntuneSubscription.md)

[Set-CMIntuneSubscription](./Set-CMIntuneSubscription.md)

