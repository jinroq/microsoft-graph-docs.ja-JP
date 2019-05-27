---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 872d736e63ce4e9119ef4cb49eb66342ebde92b5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customers = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers
    .Request()
    .GetAsync();

```