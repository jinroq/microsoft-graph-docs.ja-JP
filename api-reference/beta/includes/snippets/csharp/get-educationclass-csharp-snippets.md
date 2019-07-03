---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7e83b9e95e87c699afd7fbbe54418078263f7728
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35525908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["11023"]
    .Request()
    .GetAsync();

```