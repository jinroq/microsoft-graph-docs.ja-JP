---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 56558a4407c8626ec31b87fd28c5f3ad6f855e51
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "#4B180E";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$A$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```