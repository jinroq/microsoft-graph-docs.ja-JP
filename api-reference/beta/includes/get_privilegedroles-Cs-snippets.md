---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a0de92a6ede3449e4ebcb969ec8449b709954a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoles = await graphClient.PrivilegedRoles
    .Request()
    .GetAsync();

```