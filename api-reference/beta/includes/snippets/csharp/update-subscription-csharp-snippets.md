---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d888c1961313400a5bbc17de27af8c5a18fe73b
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846125"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ExpirationDateTime = DateTimeOffset.Parse("2016-11-22T18:23:45.9356913Z")
};

await graphClient.Subscriptions["{id}"]
    .Request()
    .UpdateAsync(subscription);

```