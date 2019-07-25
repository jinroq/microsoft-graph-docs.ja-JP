---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe6d4b1be484a4a6655f81b1dd88f40ba1d64e1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857223"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .column(5)
    .buildRequest()
    .get();

```