---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: baa61d97d1d31827299575dff7e57937eec44c2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$C$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```