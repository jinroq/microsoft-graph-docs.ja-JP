---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a3400a07145e59b4f5f0eca2d5cbca45951b4b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reminderView = await graphClient.Me
    .ReminderView('2017-06-05T10:00:00.0000000','2017-06-11T11:00:00.0000000')
    .Request()
    .GetAsync();

```