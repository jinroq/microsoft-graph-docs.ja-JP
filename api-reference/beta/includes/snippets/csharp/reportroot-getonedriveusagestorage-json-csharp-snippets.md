---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c9071a29660549199562bb897c26b09785e132b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageStorage = await graphClient.Reports
    .GetOneDriveUsageStorage("D7")
    .Request()
    .GetAsync();

```