---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ad8a5cb36b21cf6c88a9fd8000f9ba8bc4bd597
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateForward()
    .Request()
    .PostAsync();

```