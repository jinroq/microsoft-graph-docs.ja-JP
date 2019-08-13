---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23e517a494ba51471e676c95969cfcbcc77042e0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActiveUserCounts("D7")
    .Request()
    .GetAsync();

```