---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: c85dcb04ed8b011e933d95488421ffc39d936884
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Groups["{id}"].MemberOf
    .Request()
    .GetAsync();

```