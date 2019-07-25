---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45ce0f61f03a2e0a9744d5f830c9573e02178e6d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869854"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SharedDriveItem sharedDriveItem = graphClient.shares("{shareIdOrEncodedSharingUrl}")
    .buildRequest()
    .get();

```