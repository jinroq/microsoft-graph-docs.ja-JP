---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 41240d901ce6c1df025bd3745160fe9cbd619968
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserDetail = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```