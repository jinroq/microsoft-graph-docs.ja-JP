---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a60b7b738c45d1458f4518e48ce9109a7d7dd7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879365"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "subject-value";
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
message.body = body;
message.inferenceClassification = InferenceClassificationType.OTHER;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```