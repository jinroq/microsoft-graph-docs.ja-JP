---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c3502e6d39bcb3d0387f52d6abcc4d1a02d589c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .DeleteAsync();

```