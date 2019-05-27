---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a0a350786874bb7faea8c5d040cdf7fd3e430541
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```