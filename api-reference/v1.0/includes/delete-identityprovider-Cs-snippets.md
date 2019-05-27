---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2510def09068f4edb0cf9977874474c3af11b1a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .DeleteAsync();

```