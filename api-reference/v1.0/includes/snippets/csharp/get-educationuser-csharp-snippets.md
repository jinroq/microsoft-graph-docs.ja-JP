---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ebe7989c3ff5d85546aca4413499854b072c26ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{user-id}"]
    .Request()
    .GetAsync();

```