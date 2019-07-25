---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2478b99008a79a75d8b5fdee81c53561ff908f44
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Start()
    .Request()
    .PostAsync();

```