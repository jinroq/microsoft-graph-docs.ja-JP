---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d00b46323d6679e81e6d1fe3bbafd742058574f2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878813"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnenoteSectionCollectionPage sections = graphClient.me().onenote().sections()
    .buildRequest()
    .get();

```