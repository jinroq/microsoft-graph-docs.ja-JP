---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21a771591a8cccf6a0f6a90f4031be72c34885db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364805"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView()
    .range()
    .buildRequest()
    .get();

```