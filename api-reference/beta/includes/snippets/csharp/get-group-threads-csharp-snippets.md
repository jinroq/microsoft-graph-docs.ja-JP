---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d30aa90532f0dd7b3aba987b66d90d4da150003c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713628"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Threads
    .Request()
    .GetAsync();

```