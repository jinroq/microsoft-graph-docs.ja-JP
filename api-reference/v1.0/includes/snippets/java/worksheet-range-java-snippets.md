---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7bcb904ec0486ed4db9834c44fb4304ac5624050
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884351"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range('A1:B2')
    .buildRequest()
    .get();

```