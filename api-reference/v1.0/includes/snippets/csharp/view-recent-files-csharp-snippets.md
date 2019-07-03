---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 725e70c55100997bf825df7a5a017b74ac83b50e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Drive.Recent()
    .Request()
    .GetAsync();

```