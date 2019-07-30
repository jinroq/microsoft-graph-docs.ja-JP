---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 806c72db5d80cb7fb24e6cd2d668ef125c946b3d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"].Unfollow
    .Request()
    .DeleteAsync();

```