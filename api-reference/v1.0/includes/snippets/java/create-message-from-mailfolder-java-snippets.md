---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d18cd62a3cbd56314bbdcae78086a3acfa70bb2f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856350"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.receivedDateTime = "datetime-value";
message.sentDateTime = "datetime-value";
message.hasAttachments = true;
message.subject = "subject-value";
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
message.body = body;
message.bodyPreview = "bodyPreview-value";

graphClient.me().mailFolders("{id}").messages()
    .buildRequest()
    .post(message);

```