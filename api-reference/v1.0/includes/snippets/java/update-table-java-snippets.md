---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b79ec9ed4e94e7b3773a91432898281a880e1ac2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893332"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = new WorkbookTable();
workbookTable.name = "name-value";
workbookTable.showHeaders = true;
workbookTable.showTotals = true;
workbookTable.style = "style-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .patch(workbookTable);

```