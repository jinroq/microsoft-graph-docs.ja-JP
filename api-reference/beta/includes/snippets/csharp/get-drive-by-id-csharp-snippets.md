---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64e3eda9e9f75d4ccd2f5770d828837f2493076a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{driveId}"]
    .Request()
    .GetAsync();

```