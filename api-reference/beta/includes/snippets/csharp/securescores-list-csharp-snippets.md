---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 75de1e525afafa27ef985c467226d3e9100c5897
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScores = await graphClient.Security.SecureScores
    .Request()
    .Top(1)
    .GetAsync();

```