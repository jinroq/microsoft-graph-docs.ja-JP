---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f521a22dda77ecb3aa169e2dff177c2e4c97da6c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value"
};

await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .UpdateAsync(calendarGroup);

```