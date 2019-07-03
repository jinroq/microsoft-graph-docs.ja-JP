---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 661cdee88ec7b1016abae2e0975b1ce67ab10838
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472290"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .GetAsync();

```