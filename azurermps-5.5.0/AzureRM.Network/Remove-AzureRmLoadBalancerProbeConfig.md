---
Module Name: AzureRM.Network
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Remove-AzureRmLoadBalancerProbeConfig.md
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 2B15B224-E36C-454B-B6C2-F2BE032AE962
online version: https://docs.microsoft.com/en-us/powershell/module/azurerm.network/remove-azurermloadbalancerprobeconfig
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Remove-AzureRmLoadBalancerProbeConfig.md
schema: 2.0.0
---

# Remove-AzureRmLoadBalancerProbeConfig

## SYNOPSIS
Removes a probe configuration from a load balancer.

## SYNTAX

```
Remove-AzureRmLoadBalancerProbeConfig [-Name <String>] -LoadBalancer <PSLoadBalancer>
 [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmLoadBalancerProbeConfig** cmdlet removes a probe configuration from a load balancer.

## EXAMPLES

### Example 1: Remove a probe configuration from a load balancer
```
PS C:\>$loadbalancer = Get-AzureRmLoadBalancer -Name "MyLoadBalancer" -ResourceGroupName "MyResourceGroup"
PS C:> Remove-AzureRmLoadBalancerProbeConfig -Name "MyProbe" -LoadBalancer $loadbalancer
```

The first command gets the load balancer named MyLoadBalancer, and then stores it in the $loadbalancer variable.

The second command deletes the configuration named MyProbe from the load balancer in $loadbalancer.

## PARAMETERS

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with azure.

```yaml
Type: IAzureContextContainer
Parameter Sets: (All)
Aliases: AzureRmContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LoadBalancer
Specifies the load balancer that contains the probe configuration that this cmdlet removes.

```yaml
Type: PSLoadBalancer
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the probe configuration that this cmdlet removes.

```yaml
Type: String
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

### PSLoadBalancer
Parameter 'LoadBalancer' accepts value of type 'PSLoadBalancer' from the pipeline

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSLoadBalancer

## NOTES

## RELATED LINKS

[Add-AzureRmLoadBalancerProbeConfig](./Add-AzureRmLoadBalancerProbeConfig.md)

[Get-AzureRmLoadBalancer](./Get-AzureRmLoadBalancer.md)

[Get-AzureRmLoadBalancerProbeConfig](./Get-AzureRmLoadBalancerProbeConfig.md)

[New-AzureRmLoadBalancerProbeConfig](./New-AzureRmLoadBalancerProbeConfig.md)

[Set-AzureRmLoadBalancerProbeConfig](./Set-AzureRmLoadBalancerProbeConfig.md)