---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b24f66865b3df7d9b3821c0a45e7f79cb39872a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "History - World History 1",
    DisplayName = "World History Level 1"
};

await graphClient.Education.Classes["{class-id}"]
    .Request()
    .UpdateAsync(educationClass);

```