---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 80a36e2a0cbc3dfddca1156538501ad6bdd7b7a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888739"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.groups("{id}").threads("{id}").posts("{id}").attachments()
    .buildRequest()
    .get();

```