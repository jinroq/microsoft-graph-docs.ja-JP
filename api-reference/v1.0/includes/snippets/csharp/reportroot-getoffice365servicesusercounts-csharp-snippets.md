---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbbb8e9f862f74422e1e75cc19f71156ad2572a4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ServicesUserCounts('D7')
    .Request()
    .GetAsync();

```