---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d562d8d01a719e0e362f55a833f154297c72a75b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration["{id}"]
    .Request()
    .GetAsync();

```