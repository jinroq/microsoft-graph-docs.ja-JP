---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a088a6281a80b7831e94744ac44b0e14622961b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```