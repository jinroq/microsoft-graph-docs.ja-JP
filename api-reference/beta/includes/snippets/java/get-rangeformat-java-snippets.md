---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3fa85c64c77a25d7833e5ffa53d8e1e8f20afc4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874393"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .buildRequest()
    .get();

```