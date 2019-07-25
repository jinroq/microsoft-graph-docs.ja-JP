---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44ed1f03dd07fed09c89eb3263e232e3636970e4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866547"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "A1:D8";

boolean hasHeaders = False;

graphClient.me().drive().items("{id}").workbook().tables()
    .add(address,hasHeaders)
    .buildRequest()
    .post();

```