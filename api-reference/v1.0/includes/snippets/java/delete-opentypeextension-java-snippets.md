---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3f9eb72c1a3285f66c2617c89a3a062852df7606
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894411"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===").extensions("Com.Contoso.Referral")
    .buildRequest()
    .delete();

```