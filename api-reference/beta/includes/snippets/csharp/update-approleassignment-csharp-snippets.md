---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c17e63f645ee85200cd271bb8694f830d154decc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    CreationTimestamp = "2016-10-19T10:37:00Z",
    PrincipalDisplayName = "principalDisplayName-value",
    PrincipalId = "principalId-value",
    PrincipalType = "principalType-value",
    ResourceDisplayName = "resourceDisplayName-value"
};

await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .UpdateAsync(appRoleAssignment);

```