---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9702795737d7b370ed8999458513e984e0384904
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Me.Drive
    .Request()
    .GetAsync();

```