---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6aeda4f6b8388bb1ac4e9461dd6e95f534de7cf3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.Notebooks["{id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```