---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d7fed3e5838f224819bacc2ff04690a100431bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855636"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = new ScopedRoleMembership();
scopedRoleMembership.roleId = "roleId-value";
Identity roleMemberInfo = new Identity();
roleMemberInfo.id = "id-value";
scopedRoleMembership.roleMemberInfo = roleMemberInfo;

graphClient.administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .post(scopedRoleMembership);

```