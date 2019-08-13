---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 90a36027a959135380dafd58289b74326a9ea3df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserDetail = await graphClient.Reports
    .GetEmailAppUsageUserDetail("D7")
    .Request()
    .GetAsync();

```