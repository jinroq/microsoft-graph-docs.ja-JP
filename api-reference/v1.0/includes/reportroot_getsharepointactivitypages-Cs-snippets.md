---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 266c2447f5d1b2e24fa267c8687d430638f6eca0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```