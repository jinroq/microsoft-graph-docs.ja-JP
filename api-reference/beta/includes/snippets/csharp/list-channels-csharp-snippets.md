---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: f23b55e6dc51bc1030cac9c547f3cc7d151dc566
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633406"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels
    .Request()
    .GetAsync();

```