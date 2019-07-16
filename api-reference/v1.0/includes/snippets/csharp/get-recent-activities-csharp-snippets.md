---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bcaab345dffb05ab00cfda6bf015ac1a94bd2ce6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities.Recent()
    .Request()
    .GetAsync();

```