---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3dcf0ee723693f4317c8b22c9a99163858d60af3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877708"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.users("{id}").outlook().tasks("{id}").attachments()
    .buildRequest()
    .get();

```