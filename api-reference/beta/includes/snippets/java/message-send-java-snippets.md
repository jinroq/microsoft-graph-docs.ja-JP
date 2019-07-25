---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efb2781090f31c8fd0212eae2d419775e908beed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879442"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .send()
    .buildRequest()
    .post();

```