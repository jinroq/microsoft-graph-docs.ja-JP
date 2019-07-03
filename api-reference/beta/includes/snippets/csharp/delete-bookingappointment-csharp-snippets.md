---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12983dc99f7cb5cf592291fead02d5f853824f96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKqAAA="]
    .Request()
    .DeleteAsync();

```