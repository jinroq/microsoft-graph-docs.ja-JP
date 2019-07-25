---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3e256187c5f701c9b89a62ecfc5ff93b54bcb00
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891416"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = new WorkbookChartSeries();
workbookChartSeries.name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}")
    .buildRequest()
    .patch(workbookChartSeries);

```