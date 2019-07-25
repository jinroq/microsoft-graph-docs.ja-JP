---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97b80561770acfde66f61a04ec266948ed29bc54
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = new PrivilegedRoleAssignment
{
    UserId = "userId-value",
    RoleId = "roleId-value"
};

await graphClient.PrivilegedRoleAssignments
    .Request()
    .AddAsync(privilegedRoleAssignment);

```