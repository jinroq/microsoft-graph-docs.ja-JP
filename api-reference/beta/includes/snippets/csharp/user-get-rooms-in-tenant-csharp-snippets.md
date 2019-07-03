---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 702cd9ecf9e6c1d6279e5308ac5f9e1b003c6a9e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me.FindRooms()
    .Request()
    .GetAsync();

```