---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b9327c09f777a844b5ef86804b68624d6e3a963a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Adele",
    EmailAddress = "adele@relecloud.com"
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers["8bb19078-0f45-4efb-b2c5-da78b860f73a"]
    .Request()
    .UpdateAsync(bookingCustomer);

```