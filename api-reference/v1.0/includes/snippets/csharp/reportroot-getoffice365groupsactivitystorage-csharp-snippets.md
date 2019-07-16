---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c389aa78d245bbb5813ff678823555745b637775
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365GroupsActivityStorage('D7')
    .Request()
    .GetAsync();

```