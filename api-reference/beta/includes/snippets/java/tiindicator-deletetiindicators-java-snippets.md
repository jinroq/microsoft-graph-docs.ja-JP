---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b07fda38e2c21dc656fdf57eb5a26f8df9e8d2d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868235"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> valueList = new LinkedList<String>();
valueList.add("id-value1");
valueList.add("id-value2");

graphClient.security().tiIndicators()
    .deleteTiIndicators(valueList)
    .buildRequest()
    .post();

```