---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 01784e86b91cb3e0b472ec929ea2ff72ddd864e3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884407"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToNotebook(id,groupId,renameAs,siteCollectionId,siteId)
    .buildRequest()
    .post();

```