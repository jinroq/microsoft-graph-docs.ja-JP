---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc3e4d190cc84edc7be903228c5d9d8bb10cfb10
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```