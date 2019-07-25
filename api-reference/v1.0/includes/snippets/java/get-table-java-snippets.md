---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66579a9a6b6f6e1467bd66809b03662089fd1da6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890476"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .get();

```