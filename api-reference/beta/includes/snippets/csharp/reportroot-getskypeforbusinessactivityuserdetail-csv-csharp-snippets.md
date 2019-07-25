---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c0804f316621bf2b1b0b57a142a7e38ca9e6aae8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872500"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserDetail = await graphClient.Reports
    .GetSkypeForBusinessActivityUserDetail('D7')
    .Request()
    .GetAsync();

```