---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d30aa90532f0dd7b3aba987b66d90d4da150003c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Threads
    .Request()
    .GetAsync();

```