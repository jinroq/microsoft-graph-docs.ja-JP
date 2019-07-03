---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 667322331d4082546634e12b8187ceb2e1efbb4e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "displayName-value",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.Agreements["'id'"]
    .Request()
    .UpdateAsync(agreement);

```