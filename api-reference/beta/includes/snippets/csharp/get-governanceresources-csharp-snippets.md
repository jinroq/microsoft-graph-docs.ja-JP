---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 566c1d0aa99bcf0ffd5b766cf4af45b8459f1468
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.PrivilegedAccess["azureResources"].Resources
    .Request()
    .GetAsync();

```