---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e22f1248acd4be4a2dcd53ac60cfabb4a52c5a98
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892618"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartTitle workbookChartTitle = new WorkbookChartTitle();
workbookChartTitle.overlay = true;
workbookChartTitle.text = "text-value";
workbookChartTitle.visible = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").title()
    .buildRequest()
    .patch(workbookChartTitle);

```