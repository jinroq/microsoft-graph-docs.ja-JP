---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9d6b4894a37d4c48e837692e989404ad34ef57f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var metadata = "metadata-value";

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .UpdateMetadata(metadata,clientContext)
    .Request()
    .PostAsync();

```