---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a5f4369db85044aa8742c3a59df032df055a248f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867935"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.trustFramework().policies("B2C_1A_SocialAndLocalAccounts_Base")
    .buildRequest()
    .delete();

```