---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5de4df6ea5843a837df3ab1d7383384ee5713ea4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Notebooks["{id}"].Sections
    .Request()
    .GetAsync();

```