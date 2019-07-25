---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9dbb6a3524a5b4fbddb6d02c31a8e94983e1a18c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892065"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range('$B$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```