---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d82d25a09ce76cff7b8a1c84255ec1e3d706966
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String String = graphClient.education().synchronizationProfiles("{id}")
    .uploadUrl()
    .buildRequest()
    .get();

```