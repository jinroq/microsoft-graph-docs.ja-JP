---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6f7551a309c63d41051f04f5861f35e902956820
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878833"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = new Notebook();
notebook.displayName = "Notebook name";

graphClient.me().onenote().notebooks()
    .buildRequest()
    .post(notebook);

```