---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 276762a7a7b55f4ec687e78b55aa52aba3ef3ee0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464483"
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