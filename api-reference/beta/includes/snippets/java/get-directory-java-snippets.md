---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1df902afd212656c40e7abefb43f1935903ea82b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862593"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .buildRequest()
    .get();

```