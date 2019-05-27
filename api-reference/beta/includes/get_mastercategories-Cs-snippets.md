---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8b4d4c20cedb526e24a1f0b05d722c8b8d1f7050
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var masterCategories = await graphClient.Me.Outlook.MasterCategories
    .Request()
    .GetAsync();

```