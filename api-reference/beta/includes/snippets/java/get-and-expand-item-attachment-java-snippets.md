---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d905b3b0face129e30c0fdf5a1ef11e02810078
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857159"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkADA1M-zAAA=").attachments("AAMkADA1M-CJKtzmnlcqVgqI=")
    .buildRequest()
    .expand("itemattachment/item")
    .get();

```