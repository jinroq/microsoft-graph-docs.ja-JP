---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f7b863f1458fc1fea4f288c96a7a7b8228360999
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874305"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.italic = true;
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$B$1').format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```