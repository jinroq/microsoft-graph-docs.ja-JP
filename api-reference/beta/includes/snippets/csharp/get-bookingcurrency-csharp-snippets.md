---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a47e3912a9654cf08a5a6f0e3f39e228183f1b9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrency = await graphClient.BookingCurrencies["USD"]
    .Request()
    .GetAsync();

```