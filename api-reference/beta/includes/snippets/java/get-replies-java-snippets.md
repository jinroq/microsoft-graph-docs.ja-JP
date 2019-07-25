---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 187ee6d64bd2c299ee2b6c1bfcf86a0ac8009fe1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863528"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageCollectionPage replies = graphClient.chats("{id}").messages("{id}").replies()
    .buildRequest()
    .get();

```