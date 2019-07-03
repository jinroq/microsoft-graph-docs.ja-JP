---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 15d6af9dbccdf54eed689579c46dc04a200be525
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```