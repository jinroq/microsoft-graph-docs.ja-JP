---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66b16f590e48ee5c9c9bce0b5f79174eae968390
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = false,
    DisplayName = "New display name"
};

await graphClient.Applications["{id}"]
    .Request()
    .UpdateAsync(application);

```