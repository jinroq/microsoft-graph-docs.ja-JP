---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e3ec3a91137f71095e932fadc38dba18a6bbfd9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroups = await graphClient.Me.CalendarGroups
    .Request()
    .GetAsync();

```