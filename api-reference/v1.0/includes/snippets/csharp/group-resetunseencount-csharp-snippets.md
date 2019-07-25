---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c56763ca7fac873f1d2be87ac39b4c8a2fd3c682
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .ResetUnseenCount()
    .Request()
    .PostAsync();

```