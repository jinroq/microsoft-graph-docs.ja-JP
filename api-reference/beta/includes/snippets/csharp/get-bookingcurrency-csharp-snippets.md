---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a47e3912a9654cf08a5a6f0e3f39e228183f1b9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrency = await graphClient.BookingCurrencies["USD"]
    .Request()
    .GetAsync();

```