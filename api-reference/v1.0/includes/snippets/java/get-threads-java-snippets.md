---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0164d8323c5f23c7dc1f61bc4541c8c576c80887
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883719"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationThreadCollectionPage threads = graphClient.groups("{id}").conversations("{id}").threads()
    .buildRequest()
    .get();

```