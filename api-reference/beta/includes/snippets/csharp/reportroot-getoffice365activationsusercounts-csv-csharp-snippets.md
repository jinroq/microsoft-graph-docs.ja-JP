---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8b439032b3fdbd83ec6b85793d803656c0acb355
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserCounts = await graphClient.Reports.GetOffice365ActivationsUserCounts()
    .Request()
    .GetAsync();

```