---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 83ed6e76663dc14b22826fac829fd97b2758a383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserDetail = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```