---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f7eeb7c9f28036cf5f4f1800aa7087a9f74c5b58
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634154"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachment.name = "name-value";
attachment.contentBytes = "base64-contentBytes-value";

graphClient.groups("{id}").threads("{id}").posts("{id}").attachments()
    .buildRequest()
    .post(attachment);

```