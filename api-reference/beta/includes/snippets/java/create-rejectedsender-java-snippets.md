---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f4df0da2f8667b333e6fde30dd51827882dc28b6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857975"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/users/alexd@contoso.com"));

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .post(directoryObject);

```