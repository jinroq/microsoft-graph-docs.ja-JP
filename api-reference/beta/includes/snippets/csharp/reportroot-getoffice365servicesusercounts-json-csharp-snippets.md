---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2e7e023440295271833f7f11491d12ebb1261085
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ServicesUserCounts = await graphClient.Reports
    .GetOffice365ServicesUserCounts("D7")
    .Request()
    .GetAsync();

```