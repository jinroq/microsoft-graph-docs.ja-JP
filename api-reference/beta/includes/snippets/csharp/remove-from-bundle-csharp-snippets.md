---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b302e66bf1f856af18a41c252da7fbe61a9da25
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Bundles["{bundle-id}"].Children["{item-id}"]
    .Request()
    .DeleteAsync();

```