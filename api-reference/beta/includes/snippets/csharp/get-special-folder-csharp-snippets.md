---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b384b5b6742c765cae96ccf53f3d303dcc6c3ffc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Special["{name}"]
    .Request()
    .GetAsync();

```