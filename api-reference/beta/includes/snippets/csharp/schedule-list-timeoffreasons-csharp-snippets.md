---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cedf084e58b562c9cf8574106ac837853aad260
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons
    .Request()
    .GetAsync();

```