---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ed21a6053b8c92ea551acf4614ff4ce58311a2f1
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Channels["{id}"].Members["{id}"]
    .Request()
    .DeleteAsync();

```