---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2e71a139481db163d49297028d84c53788add991
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11014"].AssignmentCategories["19002"]
    .Request()
    .DeleteAsync();

```