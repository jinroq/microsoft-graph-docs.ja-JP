---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b96fd4b1b44c6c3720dd9df3158f6b6aafc372fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.Notebooks["{id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```