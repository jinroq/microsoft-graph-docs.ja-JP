---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7256b6fab723f80774692c49c814fe9a74bf146f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval
    .Request()
    .GetAsync();

```