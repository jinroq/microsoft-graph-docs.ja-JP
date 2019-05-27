---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5669fc602f905dda8d5fda80a7efe4a5f3872aa6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
    .Publish(bookingBusiness)
    .Request()
    .PostAsync();

```