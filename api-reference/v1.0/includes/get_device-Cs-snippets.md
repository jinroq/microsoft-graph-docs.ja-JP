---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cd922ccd946705b49c1a02c24511801d35e3de84
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{id}"]
    .Request()
    .GetAsync();

```