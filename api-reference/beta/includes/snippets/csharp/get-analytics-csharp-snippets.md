---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 52a38fd810ddb7b620da211155c84160f6689fcc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAnalytics = await graphClient.Drives["{drive-id}"].Items["{item-id}"].Analytics
    .Request()
    .GetAsync();

```