---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af8f54f7c4e607e409b65591811e45dd9d42ef20
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887619"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("{user-id}")
    .buildRequest()
    .delete();

```