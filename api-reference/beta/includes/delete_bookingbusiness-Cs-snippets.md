---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e6f1a2651a6c7319c8f8cabe9c26511ede97d2ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .DeleteAsync();

```