---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e88b0d444bfaa4b266b3428929739d2aadf8218
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration
    .Request()
    .GetAsync();

```