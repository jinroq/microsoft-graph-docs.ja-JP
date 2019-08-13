---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 624556c0c70431eb25500e60fb3c3ea5d70a14d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324826"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$C$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```