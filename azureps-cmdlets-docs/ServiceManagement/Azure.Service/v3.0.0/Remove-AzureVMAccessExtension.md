---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D6CE3B88-1119-4AC0-A5FC-28D0A0FA3B12
---

# Remove-AzureVMAccessExtension

## SYNOPSIS
Removes the VMAccess extension applied on a virtual machine.

## SYNTAX

```
Remove-AzureVMAccessExtension -VM <IPersistentVM> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureVMAccessExtension** cmdlet removes the VMAccess extension applied on a virtual machine.

## EXAMPLES

### Example 1: Remove a VMAccess extension from a virtual machine
```
PS C:\> Remove-AzureVMAccessExtension -VM $VM;
```

This command removes a VMAccess extension from a virtual machine.

## PARAMETERS

### -VM
Specifies the persistent virtual machine object that this cmdlet removes the VMAccess extension from.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
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

## NOTES

## RELATED LINKS

[Get-AzureVMAccessExtension](./Get-AzureVMAccessExtension.md)

[Set-AzureVMAccessExtension](./Set-AzureVMAccessExtension.md)


