---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bcb3eb3e251157ab20d2caf5e16cbe0006be6868
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```