---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ee4dad21d63e157ec2db16c69b993334d8df7c93
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891237"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRecentNotebookCollectionPage getRecentNotebooks = graphClient.me().onenote().notebooks()
    .getRecentNotebooks(true)
    .buildRequest()
    .get();

```