---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5427358dcd3be4471a5e0f19f363292bf8feb872
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469598"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reminderView = await graphClient.Me.ReminderView('2017-06-05T10:00:00.0000000','2017-06-11T11:00:00.0000000')
    .Request()
    .GetAsync();

```