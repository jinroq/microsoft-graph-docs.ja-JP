---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6463423f0c1c9e75a8e384c2748deb183fdbd205
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "edit";

String scope = "organization";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,expirationDateTime,password,message,recipientsList)
    .buildRequest()
    .post();

```