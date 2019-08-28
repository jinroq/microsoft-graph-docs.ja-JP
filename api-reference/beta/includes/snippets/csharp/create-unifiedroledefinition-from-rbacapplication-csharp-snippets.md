---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b907f6817018228086f2a1fc0c7e6ebd7f657261
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = new UnifiedRoleDefinition
{
    Description = "Update basic properties of application registrations",
    DisplayName = "Application Registration Support Administrator",
    RolePermissions = new List<UnifiedRolePermission>()
    {
        new UnifiedRolePermission
        {
            AllowedResourceActions = new List<String>()
            {
                "microsoft.directory/applications/basic/read"
            }
        }
    },
    IsEnabled = "true"
};

await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .AddAsync(unifiedRoleDefinition);

```