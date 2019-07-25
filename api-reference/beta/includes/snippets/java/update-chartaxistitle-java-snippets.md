---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a2c17c4b0836128606cbd43e307fdcda146b7f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864175"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxisTitle workbookChartAxisTitle = new WorkbookChartAxisTitle();
workbookChartAxisTitle.text = "text-value";
workbookChartAxisTitle.visible = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().title()
    .buildRequest()
    .patch(workbookChartAxisTitle);

```