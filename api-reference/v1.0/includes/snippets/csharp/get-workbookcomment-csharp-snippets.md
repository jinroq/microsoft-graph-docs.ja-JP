---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 31d1336f3fc121acc9703c4ba781ce7f31c83e4c
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookComment = await graphClient.Drive.Root.Workbook.Comments["{id}"]
    .Request()
    .GetAsync();

```