---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e1382105615d0a82dddc60e590949e21a3036e6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = await graphClient.Security.SecurityActions["{id}"]
    .Request()
    .GetAsync();

```