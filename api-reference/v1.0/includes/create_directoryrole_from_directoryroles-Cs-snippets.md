---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 734fd7fdece0c80fa973e2c979bf0c0bb182fc4d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    RoleTemplateId = "roleTemplateId-value"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```