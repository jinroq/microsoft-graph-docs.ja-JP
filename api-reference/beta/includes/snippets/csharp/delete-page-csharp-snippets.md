---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 303d24a6b10ce801e1c55c278ac9da906e886bc8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .DeleteAsync();

```