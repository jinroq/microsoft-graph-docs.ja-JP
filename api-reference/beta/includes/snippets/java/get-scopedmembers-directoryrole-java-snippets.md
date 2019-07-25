---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fdd84fa58bfe4aab2dc08960a2630cc3ba92b997
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862194"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IScopedRoleMembershipCollectionPage scopedMembers = graphClient.directoryRoles("{id}").scopedMembers()
    .buildRequest()
    .get();

```