---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a45fd4fe16d6edc85f948b56276774e49da49ff8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890343"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "test7";

String formula = "=SUM(Sheet2!$A$1+Sheet2!$A$2)";

String comment = "Comment for the named item";

graphClient.me().drive().items("{id}").workbook().names()
    .addFormulaLocal(name,formula,comment)
    .buildRequest()
    .post();

```