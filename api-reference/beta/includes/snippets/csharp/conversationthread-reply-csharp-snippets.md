---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e91951eaed9c0ef39792bd4ec47b6582912d9531
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526101"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    }
};

await graphClient.Groups["{id}"].Threads["{id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```