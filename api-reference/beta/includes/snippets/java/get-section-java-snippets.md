---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88e2d8a8dfe276a610861cde8f252be959cc3a06
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870525"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = graphClient.me().onenote().sections("{id}")
    .buildRequest()
    .get();

```