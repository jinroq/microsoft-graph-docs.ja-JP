---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 006bd9316b777233b585673243deff7d9e292bc7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var following = await graphClient.Me.Drive.Following
    .Request()
    .GetAsync();

```