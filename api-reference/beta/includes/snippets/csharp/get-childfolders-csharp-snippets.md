---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 42d8cc8ece6e8724773ace6284a27edb933348a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895548"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"].ChildFolders
    .Request()
    .GetAsync();

```