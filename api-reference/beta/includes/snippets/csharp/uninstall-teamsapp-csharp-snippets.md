---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ffffc472b27f7a6fcb59929d5a101175730fa85d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].InstalledApps["{id}"]
    .Request()
    .DeleteAsync();

```