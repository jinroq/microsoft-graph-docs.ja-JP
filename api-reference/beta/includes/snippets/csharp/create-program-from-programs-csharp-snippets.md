---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4c4c548228bb8130e5e60e5c00aa268f10b43f4a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = new Program
{
    DisplayName = "testprogram3",
    Description = "test description"
};

await graphClient.Programs
    .Request()
    .AddAsync(program);

```