---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8be11c6e6ada309679667a41ad15ead4356caf35
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKoAAA="]
    .Cancel(bookingAppointment,cancellationMessage)
    .Request()
    .PostAsync();

```