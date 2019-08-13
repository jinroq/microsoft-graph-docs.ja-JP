---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 945dddb89f0091445dd2cac4b5011bf5cb9602f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324810"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$A$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```