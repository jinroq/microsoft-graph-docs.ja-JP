---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9cc8467e5fdcff9c814612652b95bf2513998b30
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879678"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AQMkADJmMTUAAAgVZAAAA")
    .buildRequest()
    .expand("mentions")
    .get();

```