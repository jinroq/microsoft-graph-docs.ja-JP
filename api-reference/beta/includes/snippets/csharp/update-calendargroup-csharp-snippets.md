---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f521a22dda77ecb3aa169e2dff177c2e4c97da6c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486988"
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