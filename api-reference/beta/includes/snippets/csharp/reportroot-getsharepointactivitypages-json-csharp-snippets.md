---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1dc19256e8f1d2c4e70e0f13f4ab4b84354bc25f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityPages = await graphClient.Reports
    .GetSharePointActivityPages("D7")
    .Request()
    .GetAsync();

```