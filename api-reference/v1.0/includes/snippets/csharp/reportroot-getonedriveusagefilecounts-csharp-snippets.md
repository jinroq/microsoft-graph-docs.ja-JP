---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bba2ee6f96776fbd0eca01ff36863372df250055
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageFileCounts("D7")
    .Request()
    .GetAsync();

```