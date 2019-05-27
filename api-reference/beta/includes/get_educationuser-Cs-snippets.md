---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f3e97f44dcc26a0537b483d10aec5d702887f47c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["13012"]
    .Request()
    .GetAsync();

```