---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b60d6146a22b612e7f1093ad1dbdbc6ca304fec4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{id}"].Conversations
    .Request()
    .GetAsync();

```