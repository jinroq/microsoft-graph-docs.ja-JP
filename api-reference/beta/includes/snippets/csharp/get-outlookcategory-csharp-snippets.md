---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 68db4a30fc67c100faf93fdc5d6619f1575e1991
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = await graphClient.Me.Outlook.MasterCategories["de912e4d-c790-4da9-949c-ccd933aaa0f7"]
    .Request()
    .GetAsync();

```