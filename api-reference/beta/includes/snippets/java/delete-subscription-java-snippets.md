---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e69df5584684bbc0baf3aeb8112a14206d39b87
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869509"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.subscriptions("{id}")
    .buildRequest()
    .delete();

```