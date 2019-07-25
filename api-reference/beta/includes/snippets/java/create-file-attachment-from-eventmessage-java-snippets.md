---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b000fef2b16619ef9da63b19c1de8b253e0ada96
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859349"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#Microsoft.OutlookServices.FileAttachment"));
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = "contentBytes-value";

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```