---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 600ef2edb136aaa92a241b8003815ed398972310
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883861"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .post(contactFolder);

```