---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 40d149953ada10cbf26dbab553f6b17d58fa34ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders
    .Delta()
    .Request()
    .GetAsync();

```