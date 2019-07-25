---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0cfb221772fd5ce974ee25901e2520f2c55c1975
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .GetAsync();

```