---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3e9079c54c8f6ab4c7b28ad4f06931363747188
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891127"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .get();

```