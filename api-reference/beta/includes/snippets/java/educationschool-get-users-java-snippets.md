---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7cd6016522b8cfac9cce6768f8710d47f08ee380
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage users = graphClient.education().schools("10002").users()
    .buildRequest()
    .get();

```