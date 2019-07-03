---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de0e347856abdac5711bdf4d63388b1d003a4d8c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Sites["{siteId}"].Drives
    .Request()
    .GetAsync();

```