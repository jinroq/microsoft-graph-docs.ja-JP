---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c801d93e949b5aa883ab18719c1b4ca9aed6f8f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization
    .Request()
    .GetAsync();

```