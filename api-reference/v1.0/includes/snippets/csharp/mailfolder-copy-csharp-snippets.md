---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f3980b66f62545f5dc7f920ed33699d31677c93
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```