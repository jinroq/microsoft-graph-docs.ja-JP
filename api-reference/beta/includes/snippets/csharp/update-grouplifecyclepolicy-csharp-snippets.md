---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86f2fcf768faf1a77d30dd3eafc098b94b19f6c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = new GroupLifecyclePolicy
{
    GroupLifetimeInDays = 180,
    ManagedGroupTypes = "Selected",
    AlternateNotificationEmails = "admin@contoso.com"
};

await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .UpdateAsync(groupLifecyclePolicy);

```