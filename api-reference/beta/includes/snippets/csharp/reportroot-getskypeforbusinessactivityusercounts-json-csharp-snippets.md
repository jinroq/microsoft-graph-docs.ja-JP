---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd460b9b5a7b312cd24c0f36cc21ab87014473c2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessActivityUserCounts("D7")
    .Request()
    .GetAsync();

```