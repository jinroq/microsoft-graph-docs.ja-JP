---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6cdcf72e45bb8eb3d2dd5361fbc8a349682a6a8c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRule = await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZqA="]
    .Request()
    .GetAsync();

```