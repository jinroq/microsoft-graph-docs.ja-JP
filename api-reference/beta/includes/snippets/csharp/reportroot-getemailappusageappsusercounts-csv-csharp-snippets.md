---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f38fba43a737624e01894c25db015407301aeedc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageAppsUserCounts = await graphClient.Reports.GetEmailAppUsageAppsUserCounts('D7')
    .Request()
    .GetAsync();

```