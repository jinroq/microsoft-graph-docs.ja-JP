---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b7152ac5eea95eb2cf6f97d536ddaa89bd60fa0e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869902"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.creationTimestamp = "2016-10-19T10:37:00Z";
appRoleAssignment.principalDisplayName = "principalDisplayName-value";
appRoleAssignment.principalId = "principalId-value";
appRoleAssignment.principalType = "principalType-value";
appRoleAssignment.resourceDisplayName = "resourceDisplayName-value";

graphClient.servicePrincipals("{id}").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```