---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21ee4b17c5c31fd3f99c10a81989212ea23f68c1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886233"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").format().fill()
    .clear()
    .buildRequest()
    .post();

```