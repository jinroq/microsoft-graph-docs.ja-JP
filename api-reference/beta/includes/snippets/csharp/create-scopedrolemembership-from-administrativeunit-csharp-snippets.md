---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 276762a7a7b55f4ec687e78b55aa52aba3ef3ee0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = new ScopedRoleMembership
{
    RoleId = "roleId-value",
    RoleMemberInfo = new Identity
    {
        Id = "id-value"
    }
};

await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers
    .Request()
    .AddAsync(scopedRoleMembership);

```