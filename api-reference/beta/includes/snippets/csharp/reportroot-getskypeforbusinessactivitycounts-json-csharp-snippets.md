---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c9ef9e2b30737c0fd51ec712312252774e0d12b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessActivityCounts('D7')
    .Request()
    .GetAsync();

```