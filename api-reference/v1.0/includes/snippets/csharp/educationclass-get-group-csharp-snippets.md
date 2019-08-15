---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 153b0280c04a9d48467d62ead93e6dccbc372dea
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Education.Classes["{class-id}"].Group
    .Request()
    .GetAsync();

```