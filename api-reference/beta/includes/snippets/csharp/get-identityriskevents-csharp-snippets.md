---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3debe5217c9da100fb7d53bbd05722f7ae47a227
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityRiskEvents = await graphClient.IdentityRiskEvents
    .Request()
    .GetAsync();

```