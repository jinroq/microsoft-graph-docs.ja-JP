---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9378f1ec6536e3741337bda1ce100a0ba8b9706a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864682"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").channels("{id}")
    .buildRequest()
    .delete();

```