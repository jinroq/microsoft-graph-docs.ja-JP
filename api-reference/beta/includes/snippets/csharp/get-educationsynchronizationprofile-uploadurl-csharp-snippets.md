---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a6a91a4264df2bcd3dd902e7d7b73d4d420fb59d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35525907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var String = await graphClient.Education.SynchronizationProfiles["{id}"].UploadUrl()
    .Request()
    .GetAsync();

```