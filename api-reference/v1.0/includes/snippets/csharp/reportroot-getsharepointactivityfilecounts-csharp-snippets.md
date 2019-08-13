---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fa861a45d2ce750e6fbe194ed60c70c67f0ec12f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityFileCounts("D7")
    .Request()
    .GetAsync();

```