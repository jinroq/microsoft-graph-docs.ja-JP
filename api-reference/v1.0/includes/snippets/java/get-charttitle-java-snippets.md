---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 72fad8c8e47cad2b372113580ae47c9c138e6334
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891391"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartTitle workbookChartTitle = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").title()
    .buildRequest()
    .get();

```