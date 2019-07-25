---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d567ad0f507bf73ec31da4b835b65b575a8548a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"].Mentions["{id}"]
    .Request()
    .DeleteAsync();

```