---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d5c490ee8c8f09b3ba915715a6ef44d6d281f779
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityGroupCounts = await graphClient.Reports
    .GetOffice365GroupsActivityGroupCounts("D7")
    .Request()
    .GetAsync();

```