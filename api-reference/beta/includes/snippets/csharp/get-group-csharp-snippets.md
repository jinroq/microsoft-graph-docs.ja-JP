---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7980c22e1ca4152e7ea3834909392864a0bf9331
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"]
    .Request()
    .GetAsync();

```