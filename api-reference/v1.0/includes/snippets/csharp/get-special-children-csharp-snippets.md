---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 130de052d6f9e09a2f89001353900cf754bdfa06
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{special-folder-name}"].Children
    .Request()
    .GetAsync();

```