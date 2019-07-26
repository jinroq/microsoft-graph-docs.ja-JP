---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: de70c40c8727f42226e0a3e3e2fbefd3c1bb2aa5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863480"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageCollectionPage messages = graphClient.chats("{id}").messages()
    .buildRequest()
    .get();

```