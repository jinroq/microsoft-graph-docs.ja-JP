---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 26f198f915d6acbcb490632518f432ec574611a2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Education.Classes["2961761D-8094-4183-A9F6-8E36E966C7D9"].Group
    .Request()
    .GetAsync();

```