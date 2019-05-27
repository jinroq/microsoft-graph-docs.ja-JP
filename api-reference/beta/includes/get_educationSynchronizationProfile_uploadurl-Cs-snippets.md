---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a6a91a4264df2bcd3dd902e7d7b73d4d420fb59d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var String = await graphClient.Education.SynchronizationProfiles["{id}"].UploadUrl()
    .Request()
    .GetAsync();

```