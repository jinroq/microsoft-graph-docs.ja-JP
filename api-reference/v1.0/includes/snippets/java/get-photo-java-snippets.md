---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f739efc8437556b225f4a67d4a77d0924ed6175b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855074"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfilePhoto profilePhoto = graphClient.users("{id|userPrincipalName}").photo()
    .buildRequest()
    .get();

```