---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f23b55e6dc51bc1030cac9c547f3cc7d151dc566
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels
    .Request()
    .GetAsync();

```