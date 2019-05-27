---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3f21fe4aa3646cdac9f1b2e1f3a7a9b0fc10478a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = await graphClient.SchemaExtensions["graphlearn_test"]
    .Request()
    .GetAsync();

```