---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a5b8b44a59e626fc1af0dea411cc9bd7271c6aee
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataPolicyOperation dataPolicyOperation = graphClient.dataPolicyOperations("{id}")
    .buildRequest()
    .get();

```