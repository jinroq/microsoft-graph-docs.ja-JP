---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 25765918e83ccb7c3520364a2213f451eadf6edd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["46cc6179-19d0-473e-97ad-6ff84347bbbb"]
    .Restore()
    .Request()
    .PostAsync();

```