---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: fdc2d32030b31d9c79816e9b54b759a107acbd7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Invitation invitation = new Invitation();
invitation.invitedUserEmailAddress = "yyy@test.com";
invitation.inviteRedirectUrl = "https://myapp.com";

graphClient.invitations()
    .buildRequest()
    .post(invitation);

```