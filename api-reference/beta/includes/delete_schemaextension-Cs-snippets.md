---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc531ef720af87ba9a560a72b5efe39cc7fbcf1f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.SchemaExtensions["{id}"]
    .Request()
    .DeleteAsync();

```