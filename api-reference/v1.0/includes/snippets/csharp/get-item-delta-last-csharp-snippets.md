---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 857aef821e1b51555011cf3409468a75d27adaed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root.Delta('1230919asd190410jlka')
    .Request()
    .GetAsync();

```