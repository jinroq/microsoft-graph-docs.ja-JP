---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59a0854de6d37549305ac979e56818fac81b30d6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881901"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLegend workbookChartLegend = new WorkbookChartLegend();
workbookChartLegend.visible = true;
workbookChartLegend.position = "position-value";
workbookChartLegend.overlay = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").legend()
    .buildRequest()
    .patch(workbookChartLegend);

```