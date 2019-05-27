---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a5571c2af1d29ce8dff963a70bd3259c8f06f18
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroups = await graphClient.Teams["{teamId}"].Schedule.SchedulingGroups
    .Request()
    .GetAsync();

```