---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b68536bfa58d309a74c881d655586d4fbfc32fff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#Microsoft.OutlookServices.ItemAttachment"));
attachment.name = "name-value";
attachment.item = "message or event entity";

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```