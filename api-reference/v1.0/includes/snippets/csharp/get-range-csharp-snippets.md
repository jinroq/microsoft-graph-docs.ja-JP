---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8f82dc5e5ef57a926ebed63c81d118f6a05e9852
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range()
    .Request()
    .GetAsync();

```