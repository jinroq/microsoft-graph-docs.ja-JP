---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e95ebb0068827b80c36d193c2e770de159f53a6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .Renew()
    .Request()
    .PostAsync();

```