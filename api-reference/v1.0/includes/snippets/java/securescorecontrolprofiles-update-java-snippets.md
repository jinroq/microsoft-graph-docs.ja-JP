---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe28f0ee11821c43a1974d7765cf456954a34e09
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886311"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = new SecureScoreControlProfile();
secureScoreControlProfile.assignedTo = "";
secureScoreControlProfile.comment = "control is reviewed";
secureScoreControlProfile.state = "Reviewed";
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "SecureScore";
vendorInformation.providerVersion = null;
vendorInformation.subProvider = null;
vendorInformation.vendor = "Microsoft";
secureScoreControlProfile.vendorInformation = vendorInformation;

graphClient.security().secureScoreControlProfiles("NonOwnerAccess")
    .buildRequest()
    .patch(secureScoreControlProfile);

```