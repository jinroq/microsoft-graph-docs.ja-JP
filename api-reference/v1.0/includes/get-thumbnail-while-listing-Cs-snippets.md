---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18576a9a026d9dbff4c09fde918839481db3ebc7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{item-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```