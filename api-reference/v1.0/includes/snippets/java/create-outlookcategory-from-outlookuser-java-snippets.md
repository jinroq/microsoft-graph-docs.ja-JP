---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bad2b1fae7a93b8ec4507acfa3f4ae8d6652ff1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891252"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = new OutlookCategory();
outlookCategory.displayName = "Project expenses";
outlookCategory.color = CategoryColor.PRESET9;

graphClient.me().outlook().masterCategories()
    .buildRequest()
    .post(outlookCategory);

```