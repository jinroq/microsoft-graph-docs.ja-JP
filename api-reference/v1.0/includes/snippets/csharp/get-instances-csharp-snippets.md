---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d229f6306cee32267c60590661d8427ebd1dded1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2019-04-08T09:00:00.0000000"),
    new QueryOption("endDateTime", "2019-04-30T09:00:00.0000000")
};

var instances = await graphClient.Me.Events["AAMkAGUzYRgWAAA="].Instances
    .Request( queryOptions )
    .Select( e => new {
             e.Subject,
             e.BodyPreview,
             e.SeriesMasterId,
             e.Type,
             e.Recurrence,
             e.Start,
             e.End 
             })
    .GetAsync();

```