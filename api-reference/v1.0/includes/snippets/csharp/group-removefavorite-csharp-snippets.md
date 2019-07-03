---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6d133bfd8fa4cd5454e23c0d883cd3d0fb163e7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .RemoveFavorite()
    .Request()
    .PostAsync();

```