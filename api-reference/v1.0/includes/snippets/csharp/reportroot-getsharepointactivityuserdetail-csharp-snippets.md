---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 100d672ae20008834348c31d54814dbf41a988ac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserDetail("D7")
    .Request()
    .GetAsync();

```