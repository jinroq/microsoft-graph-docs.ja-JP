---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d038bd79708e24b81e814f230370d42345b0366
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountDetail = await graphClient.Reports
    .GetOneDriveUsageAccountDetail("D7")
    .Request()
    .GetAsync();

```