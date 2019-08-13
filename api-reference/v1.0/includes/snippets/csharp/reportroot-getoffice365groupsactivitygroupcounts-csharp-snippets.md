---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8c1b32325c0c7203b7c26ade81eaff2578a1672
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityGroupCounts("D7")
    .Request()
    .GetAsync();

```