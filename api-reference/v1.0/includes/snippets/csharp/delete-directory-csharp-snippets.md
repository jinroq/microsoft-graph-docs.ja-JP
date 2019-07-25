---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef1d0938090343a4388b9249921fe0a72d538f40
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Request()
    .DeleteAsync();

```