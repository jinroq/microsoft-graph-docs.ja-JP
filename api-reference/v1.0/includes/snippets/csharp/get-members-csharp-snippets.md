---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87ea6a9955decfca7ce6cadec6c4e5b1c3e6e45d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{id}"].Members
    .Request()
    .GetAsync();

```