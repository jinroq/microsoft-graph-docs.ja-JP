---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1bde40d4f8dba0b84ea566017e565a487436c95e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325844"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("workbook-session-id", "{session-id}"));

graphClient.me().drive().items("{id}").workbook()
    .refreshSession()
    .buildRequest( requestOptions )
    .post();

```