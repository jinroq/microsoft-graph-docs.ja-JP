---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8fd5bdf2e1e25a1cc2d31835a424798bccbaa85f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863589"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageHostedContentCollectionPage hostedContents = graphClient.chats("{id}").messages("{id}").hostedContents()
    .buildRequest()
    .get();

```