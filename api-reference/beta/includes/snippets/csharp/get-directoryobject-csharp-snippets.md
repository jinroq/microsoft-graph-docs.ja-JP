---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b81c390c250d4f1105535bdb7eb407bd70a1d030
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{id}"]
    .Request()
    .GetAsync();

```