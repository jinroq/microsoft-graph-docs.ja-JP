---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 34b448da31da5368d723339d7e9b6129f5dbbd00
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = true,
    DisplayName = "Display name"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```