---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ecb632ca44e324bb42b987ce085280184050175
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive
    .Search("{search-query}")
    .Request()
    .GetAsync();

```