---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 36768d24208b36f2e81f04d6d595223a1ef69048
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports
    .GetAzureADApplicationSignInSummary("D7")
    .Request()
    .GetAsync();

```