---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 844edd6322b7bc3d8dac7828672994dd91203421
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityGroupCounts("D7")
    .Request()
    .GetAsync();

```