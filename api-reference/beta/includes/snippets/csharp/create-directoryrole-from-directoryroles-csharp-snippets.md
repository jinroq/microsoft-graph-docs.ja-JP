---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88deacf3d76679a76da39083f345dc7e794d7064
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    Description = "description-value",
    DisplayName = "displayName-value",
    RoleTemplateId = "roleTemplateId-value"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```