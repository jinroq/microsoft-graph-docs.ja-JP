---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 5d0e56df3ee0bbb39c89be8fe56d3160165f9910
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882807"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("displayName,givenName,postalCode")
    .get();

```