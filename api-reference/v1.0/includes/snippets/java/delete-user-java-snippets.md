---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: b323ebbc55e54b5497678bd5135e032364ea1a47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{user-id}")
    .buildRequest()
    .delete();

```