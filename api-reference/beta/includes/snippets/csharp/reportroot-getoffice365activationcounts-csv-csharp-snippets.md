---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d97a7e041480ae2737043cddf2c6b559f3b69572
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464548"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationCounts = await graphClient.Reports.GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```