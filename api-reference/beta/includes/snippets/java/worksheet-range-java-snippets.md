---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a69f086a0a8bb9bcf385c97b22b2ff876a227b4b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866124"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "address-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range()
    .buildRequest()
    .post();

```