---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1869c2843504f59d38cd478651fb9a60deae42ec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875894"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = new PrivilegedApproval();
privilegedApproval.userId = "userId-value";
privilegedApproval.roleId = "roleId-value";
privilegedApproval.approvalType = "approvalType-value";
privilegedApproval.approvalState = ApprovalState.PENDING;
privilegedApproval.approvalDuration = "datetime-value";

graphClient.privilegedApproval()
    .buildRequest()
    .post(privilegedApproval);

```