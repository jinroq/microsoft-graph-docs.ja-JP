---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f0a301884763f1a0cd82d38cd85a3ec7ce6e1164
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880276"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest()
    .delete();

```