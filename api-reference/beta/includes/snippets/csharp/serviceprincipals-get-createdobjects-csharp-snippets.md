---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99e198b94e9018f1c88f913ef068dfc7a5678c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.ServicePrincipals["{id}"].CreatedObjects
    .Request()
    .GetAsync();

```