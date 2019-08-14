---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dfc9d765e635928943291ff9ed8221e167b36c2c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372759"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```