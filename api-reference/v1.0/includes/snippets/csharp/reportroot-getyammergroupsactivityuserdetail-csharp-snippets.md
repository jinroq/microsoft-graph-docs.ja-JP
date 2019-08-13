---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9182df426f75e468a05c2f01169d2471d1196a31
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320224"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityDetail("D7")
    .Request()
    .GetAsync();

```