---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9d6b4894a37d4c48e837692e989404ad34ef57f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503978"
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