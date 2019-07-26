---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 07bfaba11be1239f4827dc3997d3c47e4c93a642
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889502"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("b320ee12-b1cd-4cca-b648-a437be61c5cd")
    .buildRequest()
    .select("allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount")
    .get();

```