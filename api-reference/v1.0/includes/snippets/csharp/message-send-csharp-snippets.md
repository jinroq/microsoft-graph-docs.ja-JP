---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 09d143dbf9c7b14c2180817bb8b2dbc50284feb0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Send()
    .Request()
    .PostAsync();

```