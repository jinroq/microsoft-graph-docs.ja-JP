---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6db4fc633674d05365f48838503b9709e3b734a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityCounts = await graphClient.Reports
    .GetYammerGroupsActivityCounts("D7")
    .Request()
    .GetAsync();

```