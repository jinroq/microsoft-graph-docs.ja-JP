---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: df4dde836ad98b32638caa830cd8711411ffbde2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders
    .Request()
    .AddAsync(mailFolder);

```