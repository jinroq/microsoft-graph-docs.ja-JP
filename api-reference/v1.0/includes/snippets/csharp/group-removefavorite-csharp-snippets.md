---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6d133bfd8fa4cd5454e23c0d883cd3d0fb163e7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .RemoveFavorite()
    .Request()
    .PostAsync();

```