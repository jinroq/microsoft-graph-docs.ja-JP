---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 0949f9448e42efa2818a0c14d7a6cd83b2ef61fb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887890"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.me().drive()
    .buildRequest()
    .get();

```