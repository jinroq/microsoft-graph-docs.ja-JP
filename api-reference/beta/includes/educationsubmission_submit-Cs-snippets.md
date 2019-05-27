---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ac9e4b078a9cf2720bad1b941d3cb559b6e2efe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Submit()
    .Request()
    .PostAsync();

```