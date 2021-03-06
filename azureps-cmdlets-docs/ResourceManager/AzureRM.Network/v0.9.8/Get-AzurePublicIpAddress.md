---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 7F4739DD-9515-4CA8-9B06-61AA8D39EEE3
---

# Get-AzurePublicIpAddress

## SYNOPSIS
Gets a public IP address.

## SYNTAX

```
Get-AzurePublicIpAddress [-Name <String>] [-ResourceGroupName <String>] [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzurePublicIPAddress** cmdlet gets one or more public IP addresses in a resource group.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Name
Specifies the name of the public IP address to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ResourceName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies an Azure profile.

```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the public IP address to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzurePublicIpAddress](./New-AzurePublicIpAddress.md)

[Remove-AzurePublicIpAddress](./Remove-AzurePublicIpAddress.md)

[Set-AzurePublicIpAddress](./Set-AzurePublicIpAddress.md)


