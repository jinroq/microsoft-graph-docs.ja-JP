---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e19d71d43c52dd83a023d53ad0441286ee1c199
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879535"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.referenceAttachment"));
attachment.name = "Personal pictures";
attachment.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachment.providerType = "oneDriveConsumer";
attachment.permission = "Edit";
attachment.isFolder = "True";

graphClient.me().messages("AAMkAGE1M88AADUv0uFAAA=").attachments()
    .buildRequest()
    .post(attachment);

```