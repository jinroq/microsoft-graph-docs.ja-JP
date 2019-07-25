---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a958b4328166e105ad2b16441d545d32030d6efb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = True;

graphClient.me().events("{id}")
    .decline(comment,sendResponse)
    .buildRequest()
    .post();

```