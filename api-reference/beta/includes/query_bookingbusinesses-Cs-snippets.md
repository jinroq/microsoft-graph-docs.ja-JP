---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 25b878914d55d3a0b6152ae3c12c60c6db3a2673
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("query", "Adventure")
};

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request( queryOptions )
    .GetAsync();

```