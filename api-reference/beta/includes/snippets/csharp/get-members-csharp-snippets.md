---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 900ffa40398aae5aee9592ff9d76bf2178aa98f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["11016"].Members
    .Request()
    .GetAsync();

```