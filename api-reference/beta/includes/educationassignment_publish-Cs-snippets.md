---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e052f9abc42dcdd357eaeef31f818b72cdca9957
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"]
    .Publish()
    .Request()
    .PostAsync();

```