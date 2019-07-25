---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: caca9d0f0f0eaca3ec2d34d003b97cd473c3748f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858197"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMembers = graphClient.groups("{id}").transitiveMembers()
    .buildRequest()
    .get();

```