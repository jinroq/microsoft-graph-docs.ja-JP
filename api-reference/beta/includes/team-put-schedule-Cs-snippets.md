---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1079684b3063183e2e93b2ceb9b7e899e2d186b8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = new Schedule
{
    Enabled = true,
    TimeZone = "America/Chicago"
};

await graphClient.Teams["{teamId}"].Schedule
    .Request()
    .PutAsync(schedule);

```