---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3b18d39708d1fda22577c1e6fd9c24b569f02c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```