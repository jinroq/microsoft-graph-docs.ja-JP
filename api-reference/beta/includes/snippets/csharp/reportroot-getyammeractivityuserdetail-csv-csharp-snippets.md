---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 627a877b6da9510b772424eecc738492f4a4963c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserDetail = await graphClient.Reports.GetYammerActivityUserDetail('D7')
    .Request()
    .GetAsync();

```