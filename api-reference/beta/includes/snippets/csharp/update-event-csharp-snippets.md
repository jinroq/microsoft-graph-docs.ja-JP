---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3df7242cc7dc9845289883d3bf3897af9c7acd01
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    OriginalStartTimeZone = "originalStartTimeZone-value",
    OriginalEndTimeZone = "originalEndTimeZone-value",
    ResponseStatus = new ResponseStatus
    {
        Response = ResponseType.None,
        Time = "2016-10-19T10:37:00Z"
    },
    Recurrence = null,
    Uid = "iCalUId-value",
    ReminderMinutesBeforeStart = 99,
    IsReminderOn = true
};

await graphClient.Me.Events["{id}"]
    .Request()
    .UpdateAsync(@event);

```