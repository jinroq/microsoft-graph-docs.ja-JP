---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ac643ad2212bbbf56c55c89cf4f59f07e223623
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706280"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Groups["{groupId}"].Drives
    .Request()
    .GetAsync();

```