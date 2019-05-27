---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a4dd2963e90c4c3b9983aab9d786fa9276c2afa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["AAMkAGI2THk0AAA="]
    .Request()
    .GetAsync();

```