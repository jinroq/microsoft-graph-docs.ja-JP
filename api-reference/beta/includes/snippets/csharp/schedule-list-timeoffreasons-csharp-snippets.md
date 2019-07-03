---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cedf084e58b562c9cf8574106ac837853aad260
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons
    .Request()
    .GetAsync();

```