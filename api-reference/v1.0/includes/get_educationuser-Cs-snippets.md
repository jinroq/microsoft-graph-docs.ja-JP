---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ebe7989c3ff5d85546aca4413499854b072c26ac
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{user-id}"]
    .Request()
    .GetAsync();

```