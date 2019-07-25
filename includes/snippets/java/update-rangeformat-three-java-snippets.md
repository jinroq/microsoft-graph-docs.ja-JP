---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 787d730f86e5e16bba8f7a95acb9783d07cce7f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857418"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135;
workbookRangeFormat.horizontalAlignment = "Right";
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$C$1').format()
    .buildRequest()
    .patch(workbookRangeFormat);

```