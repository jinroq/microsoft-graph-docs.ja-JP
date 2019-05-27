---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 77981e93f43fc4cf9a0a0fcdd94fc268524b8cb2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-name}"]
    .Verify()
    .Request()
    .PostAsync();

```