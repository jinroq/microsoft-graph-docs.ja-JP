---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a6f69fa522b30fb8434301d44109f702ffc38c36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00.0000000"),
    new QueryOption("endDateTime", "2017-01-07T19:00:00.0000000")
};

var calendarView = await graphClient.Me.Calendar.CalendarView
    .Request( queryOptions )
    .GetAsync();

```