---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: afc31a36c4e0a89a0f3151a6a1328f19b0d17381
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.DirectoryRoles
    .Delta()
    .Request()
    .GetAsync();

```