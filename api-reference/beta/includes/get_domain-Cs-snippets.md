---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4bf9214aaf694fc1ebfb4a87423825ea72cab649
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = await graphClient.Domains["contoso.com"]
    .Request()
    .GetAsync();

```