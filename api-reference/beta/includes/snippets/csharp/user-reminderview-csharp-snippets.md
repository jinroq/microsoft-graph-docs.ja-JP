---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5427358dcd3be4471a5e0f19f363292bf8feb872
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reminderView = await graphClient.Me.ReminderView('2017-06-05T10:00:00.0000000','2017-06-11T11:00:00.0000000')
    .Request()
    .GetAsync();

```