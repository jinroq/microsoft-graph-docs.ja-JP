---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 832c66862a9eb029d1a5fc1d62dee261eb5de107
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers["80b5ddda-1e3b-4c9d-abe2-d606cc075e2e"]
    .Request()
    .DeleteAsync();

```