---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a094c980539f75a2d663cecc77cbe2f00c28479
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Me.Drives
    .Request()
    .GetAsync();

```