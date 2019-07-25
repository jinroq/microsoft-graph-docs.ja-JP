---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 33833c4c230018c8803a3d497d0976b219d1884b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply()
    .buildRequest()
    .post();

```