---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8f59ed646d1e30fa4a4cff6eceeb56fcfeb927e0
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Items["{bundle-id}"]
    .Request()
    .DeleteAsync();

```