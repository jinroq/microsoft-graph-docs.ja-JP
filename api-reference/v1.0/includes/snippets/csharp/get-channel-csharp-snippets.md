---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8962445fc41eb169eff91bd17c6c88e7e693682
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .GetAsync();

```