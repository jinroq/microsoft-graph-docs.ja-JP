---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef50eb61e92f955b1d39dd657af6b91b53eec763
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879121"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String webUrl = "webUrl value";

graphClient.me().onenote().notebooks()
    .getNotebookFromWebUrl(webUrl)
    .buildRequest()
    .post();

```