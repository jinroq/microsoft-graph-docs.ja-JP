---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a3f953697a333f17e730a818d6b892a93872171
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .DeleteAsync();

```