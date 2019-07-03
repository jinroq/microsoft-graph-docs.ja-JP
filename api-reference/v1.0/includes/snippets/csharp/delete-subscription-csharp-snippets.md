---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4794d8788d3d40150f96f03065ef5f486232c699
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["{id}"]
    .Request()
    .DeleteAsync();

```