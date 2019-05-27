---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7af19f122901e1b7ab213989b9fd6e1a5f72a5fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443853"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Notebooks["{id}"]
    .CopyNotebook(groupId,renameAs,notebookFolder,siteCollectionId,siteId)
    .Request()
    .PostAsync();

```