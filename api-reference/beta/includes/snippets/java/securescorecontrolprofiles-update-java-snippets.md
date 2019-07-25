---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d52bd9f8ce98d0552b85cfbff25f9888c257f159
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870356"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = new SecureScoreControlProfile();
secureScoreControlProfile.controlStateUpdates = "controlStateUpdates-value";

graphClient.security().secureScoreControlProfiles("AdminMFA")
    .buildRequest()
    .patch(secureScoreControlProfile);

```