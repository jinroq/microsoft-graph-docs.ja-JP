---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d824175e32957c3846b5c95796e22a051b6d948
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.programControls("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .delete();

```