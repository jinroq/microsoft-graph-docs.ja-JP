---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 513f0ca0e522d95bd31025bab61fe6d3033cb66e
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    CreationTimestamp = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    PrincipalDisplayName = "principalDisplayName-value",
    PrincipalId = Guid.Parse("principalId-value"),
    PrincipalType = "principalType-value",
    ResourceDisplayName = "resourceDisplayName-value"
};

await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .UpdateAsync(appRoleAssignment);

```