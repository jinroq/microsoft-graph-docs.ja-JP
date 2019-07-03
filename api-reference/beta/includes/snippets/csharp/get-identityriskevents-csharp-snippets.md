---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3debe5217c9da100fb7d53bbd05722f7ae47a227
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503680"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityRiskEvents = await graphClient.IdentityRiskEvents
    .Request()
    .GetAsync();

```