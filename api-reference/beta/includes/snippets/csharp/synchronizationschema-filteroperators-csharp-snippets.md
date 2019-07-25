---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b666907f3d7993c3be38c3413fad67ae51dde8e3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterOperators = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema
    .FilterOperators()
    .Request()
    .GetAsync();

```