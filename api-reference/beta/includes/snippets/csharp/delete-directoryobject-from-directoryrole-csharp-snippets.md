---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4002b673791aebe1f85b7d5aa36c1e7d3f77ca46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directoryroles["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```