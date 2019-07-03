---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 053da63945be69e296ea066fe0a739bd9e9ab24e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var duration = "duration-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoles["{id}"]
    .SelfActivate(reason,duration,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```