---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 558f05029b98369630253d10b27489683ceb54f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885029"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .get();

```