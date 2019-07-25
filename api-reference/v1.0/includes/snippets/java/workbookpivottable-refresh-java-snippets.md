---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c2845fa6181f20f0c0dc76fe8132f6ccd220ed4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884581"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .refresh()
    .buildRequest()
    .post();

```