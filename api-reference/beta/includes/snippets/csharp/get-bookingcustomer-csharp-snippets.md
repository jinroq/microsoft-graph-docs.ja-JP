---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88b1c490792047e4c9a25fcec833912ab5cc984f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers["8bb19078-0f45-4efb-b2c5-da78b860f73a"]
    .Request()
    .GetAsync();

```