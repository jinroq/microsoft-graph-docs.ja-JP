---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: be134ebdd3bb721106176d97135e31aad27e0ae2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864147"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "ColumnStacked";

String sourceData = "A1:B1";

String seriesBy = "Auto";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts()
    .add(type,sourceData,seriesBy)
    .buildRequest()
    .post();

```