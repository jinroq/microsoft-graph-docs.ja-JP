---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc531ef720af87ba9a560a72b5efe39cc7fbcf1f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.SchemaExtensions["{id}"]
    .Request()
    .DeleteAsync();

```