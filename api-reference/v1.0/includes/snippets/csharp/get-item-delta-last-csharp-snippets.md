---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d230ad94354fec54b9972313c89ff3c567949ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root
    .Delta("1230919asd190410jlka")
    .Request()
    .GetAsync();

```