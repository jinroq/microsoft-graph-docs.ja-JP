---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 78109d5ac5ad2aba8fdb694fc0987f3af3bc964e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```