---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f1cd9bcc652659b1e8ba2bdd3b3ef61baf6e6b5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.GivenName,
             e.PostalCode 
             })
    .GetAsync();

```