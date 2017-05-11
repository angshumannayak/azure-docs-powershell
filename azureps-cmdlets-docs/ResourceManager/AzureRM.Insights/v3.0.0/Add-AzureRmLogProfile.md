---
external help file: Microsoft.Azure.Commands.Insights.dll-Help.xml
ms.assetid: 18D5B95E-4CF1-4C79-AE8B-9F4DA49B46A9
online version: 
schema: 2.0.0
---

# Add-AzureRmLogProfile

## SYNOPSIS
Creates a log profile. This profile will be used to archive the activity log to a storage account or stream them to an Azure event hub. Only standard storage account (premium storage account is not supported) both ARM and Classic are supported. If it's logged to storage account the cost of storing this activity log is billed at normal storage rates. 

## SYNTAX

```
Add-AzureRmLogProfile -Name <String> [-StorageAccountId <String>] [-ServiceBusRuleId <String>]
 [-RetentionInDays <Int32>] -Locations <System.Collections.Generic.List`1[System.String]>
 [-Categories <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmLogProfile** cmdlet creates a log profile.

## EXAMPLES

### 1:
### Example 1 : Add a new log profile to export activity logs to a storage account 
```yaml
Add-AzureRmLogProfile -Locations "West US" -Name ExportLogProfile -StorageAccountId /subscriptions/40gpe80s-9sb7-4f07-9042-b1b6a92ja9fk/resourceGroups/activitylogRG/providers/Microsoft.Storage/storageAccounts/activitylogstorageaccount 
```

## PARAMETERS

### -Categories
Specifies the list of categories.
  
```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Locations
Specifies the list of locations.
Specifies the location of the log profile.

Valid values: Run below cmdlet   to get the latest list of locations. 
```yaml
Get-AzureLocation | Select DisplayName
```

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RetentionInDays
Specifies the retention policy, in days. This is the number of days the logs are preserved in the storage account specified. To retain the data forever set this 0. If it's not specified, then it defaults to 0 which is retain for ever. 

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```


### -ServiceBusRuleId
Specifies the ID of the Service Bus rule.

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

### -StorageAccountId
Specifies the ID of the Storage account. ID is the fully qualified Resource ID of the storage account for example  
```yaml
/subscriptions/40gpe80s-9sb7-4f07-9042-b1b6a92ja9fk/resourceGroups/activitylogRG/providers/Microsoft.Storage/storageAccounts/activitylogstorageaccount
```

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
### -Example 

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmLogProfile](./Get-AzureRmLogProfile.md)

[Remove-AzureRmLogProfile](./Remove-AzureRmLogProfile.md)


